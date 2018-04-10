## These instructions haven't yet been tested - they are a framework.

Make sure you have vim version 8.0 or higher.
*  On macOS you can use ```brew install vim``` and then insert ```export PATH=/usr/local/Cellar/vim/8.0.1650_1/bin:$PATH``` into your ```~/.bashrc``` file.

Install the vim package manager:    https://github.com/tpope/vim-pathogen

Install the vlime package:  
https://github.com/l04m33/vlime

Run vlime from Cando/Clasp using: ```(load "<vlime-path>/lisp/start-vlime.lisp")```

Add ```syntax on``` to the top of your .vimrc file.

Use \cc to connect.

Use \ss to evaluate.