#The Clasp build system.

It uses a combination of make files "makefile" in each directory: clasp/, clasp/src, clasp/src/gctools, clasp/src/core ...  and boost build jam files.

Important files:

1. clasp/makefile.inc - this is included in other makefiles in other directories
1. clasp/makefile - top level makefile
1. clasp/src/makefile - invokes make in source directories
1. clasp/src/XXX/makefile - where XXX is gctools, core, clbind, asttooling, main etc.
1. clasp/Jamroot.jam - top level jam file
1. clasp/src/XXX/Jamfile.jam - source directory jam files

Important targets:
* make prebuild  - Performs symbol scraping, class scraping, and Google pump file compilation
* bjam targets

----------------------------------------------------------------------
----------------------------------------------------------------------
## Source directories:
- src/gctools/
- src/core/
- src/clbind/
- src/llvmo/
- src/cffi/
- src/asttooling/
- src/serveEvent/
- src/sockets/
- src/mpip/
- src/main/

----------------------------------------------------------------------
----------------------------------------------------------------------
## Google pump

Google pump.py is a python program that converts .pmp files into header files.
".pmp" files contain a description of C++ template code that gets expanded into lots of repetative C++ template code.
Every .pmp file needs to have google pump run on it.

They are build using a %.h : %.pmp rule in clasp/makefile.inc.  The generated header files are dependencies of the "sub-prebuild" target in clasp/src/clbind/makefile and clasp/src/core/makefile.

These are the current active .pmp files:

- src/clbind/clbind_constructor_functoids.pmp
- src/clbind/clbind_functoids.pmp
- src/clbind/clbind_methoids.pmp
- src/clbind/clbind_static_members.pmp
- src/clbind/constructors.pmp
- src/core/applyToActivationFrame.pmp
- src/core/external_wrappers_indirect_methoids.pmp
- src/core/wrappers_functoids.pmp
- src/core/wrappers_methoids.pmp

They generate header files with the same name suffixed with ".h" and they are written into the clasp/include/clbind/generated/ and clasp/include/core/generated/ directories.

This process doesn't depend on anything, only if one of these .pmp files changes does pump need to be run on the file.
The pump.py code is in clasp/src/common/pump.py



----------------------------------------------------------------------
----------------------------------------------------------------------
##Symbol scraping

In each source directory XXX is a file called: "XXX/include/symbols_scraped_inc.h"
it lists the names and packages of Common Lisp SYMBOLs that are accessible to C++ as symbols with the names prefixed with "_sym_" ie: "_sym_list".

Before any files are built and at the beginning of every build the following script is run:
python src/common/symbolScraper.py *.cc include/*.h

In each of the source directories XXX is a include/ symbolic link to a clasp/include/clasp/XXX directory that contains header files for each source directory.

The script extracts macros named the following from all of these files:
SYMBOL_EXPORT_SC_(pkg,name)     // exported symbol in pkg
SYMBOL_SC_(pkg,name)            // internal symbol in pkg
LISP_CLASS(...)
...others...

It builds a symbol table and compares it to the contents of symbols_scraped_inc.h,
if there are any differences (symbols added, removed or changed) then it generates a new symbols_scraped_inc.h file.

The symbols_scraped_inc.h file is included by almost every .cc file so that they have access to Common Lisp symbols without having to mess around with strings.

To summarize:
1) Symbol scraping scrapes all of the .cc files and may or may not generate a new symbols_scraped_inc.h file
2) .cc files #include the symbols_scraped_inc.h file

----------------------------------------------------------------------
----------------------------------------------------------------------
##Register classes

This searches through the C++ header and source files for definitions of C++ classes that will be exposed to Common Lisp.

/usr/bin/python /Users/meister/Development/clasp/src/common/registerClasses.py include/generated/initClasses_inc.h include/*Package.h include/*.h *.h *.cc 2> registerClasses.log

Searches through all header files looking for macros like:
LISP_CLASS(...)

It populates the file XXX/include/generated/initClasses_inc.h with code that exposes these C++ classes to Common Lisp


----------------------------------------------------------------------
----------------------------------------------------------------------





See src/lisp/Jamfile.jam
Copy src/lisp source tree (*.l *.lsp *.lisp *.sh) to $(APPRES-LISP)

src/core/bin/boehm/clang-darwin-4.2.1/release/link-static/core_scrape_flag.h
src/cffi/bin/boehm/clang-darwin-4.2.1/release/link-static/cffi_scrape_flag.h

Build .cc files in main

scraped ../../src/gctools/bin/boehm/clang-darwin-4.2.1/release/link-static/gctools_scrape_flag.h
	touch ../../src/gctools/bin/boehm/clang-darwin-4.2.1/release/link-static/gctools_scrape_flag.h
scraped ../../src/sockets/bin/boehm/clang-darwin-4.2.1/release/link-static/sockets_scrape_flag.h
	touch ../../src/sockets/bin/boehm/clang-darwin-4.2.1/release/link-static/sockets_scrape_flag.h
scraped ../../src/serveEvent/bin/boehm/clang-darwin-4.2.1/release/link-static/serveEvent_scrape_flag.h
	touch ../../src/serveEvent/bin/boehm/clang-darwin-4.2.1/release/link-static/serveEvent_scrape_flag.h
scraped ../../src/clbind/bin/boehm/clang-darwin-4.2.1/release/link-static/clbind_scrape_flag.h
	touch ../../src/clbind/bin/boehm/clang-darwin-4.2.1/release/link-static/clbind_scrape_flag.h
