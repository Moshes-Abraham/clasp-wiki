With Xcode 11 apple no longer provides the standard headers in /usr/include and 
`/Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg`might´, that copies the headers might no longer be shipped.

To use the standard headers I believe the following has to be done:
In https://github.com/clasp-developers/clasp/blob/dev/wscript#L1040
replace 
```
    c++cfg.env.append_value('INCLUDES', ['/usr/include'] )
````
with
```c++
    cfg.env.append_value('INCLUDES', ['/Library/Developer/CommandLineTools/usr/include/c++/v1'] )
    cfg.env.append_value('INCLUDES', ['/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include'] )
````

Additionally the are now warnings about nullability errors like:
```c++
In file included from ../../src/fork-server/fork-client.c:14:
/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include/signal.h:69:21: warning: pointer is missing a nullability type specifier (_Nonnull, _Nullable, or _Null_unspecified) [-Wnullability-completeness]
extern __const char *__const sys_signame[NSIG];
                    ^
/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include/signal.h:69:21: note: insert '_Nullable' if the pointer may be null
extern __const char *__const sys_signame[NSIG];
                    ^
                      _Nullable 
/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include/signal.h:69:21: note: insert '_Nonnull' if the pointer should never be null
extern __const char *__const sys_signame[NSIG];
                    ^
                      _Nonnull 
````

These should disappear by adding
```c++
    cfg.env.append_value('CXXFLAGS', ['-Wno-nullability-completeness'] )
    cfg.env.append_value('CXXFLAGS', ['-Wno-nonnull'] )
`````
to the cxxflags after https://github.com/clasp-developers/clasp/blob/dev/wscript#L1075

For whatever reason, that only worked with the headers from xcode 10.X and not with the headers from Xcode 11.X 