### Movement

| command | description |
| ------- | ----------- |
| control-f | page down |
| control-b | page up |
| control-u | half page down |
| control-d | half page up |
| # | go to previous occurrence of the string under the cursor |
| * | go to next occurrence of the string under the cursor |
| ( ) | backward / forward by sentence |
| { } | backward / forward by block (blank lines) |
| gg | go to top of file |
| G | go to bottom of file |
| zz | center the screen around your cursor |
| ZZ or :wq | save + quit |
| db | delete word backwards |
| control-w | delete word backwards in insert mode |
| control-u | delete from the beginning of the line to the cursor in insert mode |
| m[a-z] | place a mark |
| m[A-Z] | place a global mark |
| `[a-zA-Z] | jump to mark |
| `` | jump to previous mark |
| m" | jump to position when last editing the file |
| m[ | start of last change |
| m] | end of last change |
<!-- ` -->

### Search
| command | description |
| ------- | ----------- |
| / | search |
| ? | search backwards |

### Buffers
| command | description |
| ------- | ----------- |
| :ls or :buffers | list buffers |
| :bd | close buffer without quitting vim |
| :bn | next buffer |
| :bp | previous buffer |
| :tabe | open file in a new tab |
| :e <filename> | open file |

### Splitting the window
| command | description |
| ------- | ----------- |
| :split | split horizontally |
| :vsp or :vsplit | split vertically |
| control-w w | move to the other window |
| control-w <arrow key or hjkl> | move to window in that direction |
| control-w o | close other windows |


### Other

| command | description |
| ------- | ----------- |
| u | undo |
| control-r | redo |
| set expandtab tabstop=4 shiftwidth=4 | set tab size |
| gg=G | reindent the file |
| :so ~/.vimrc | reload .vimrc file |
| :set incsearch hlsearch | turn on incremental search and highlight search |
| diw | delete the whole word your cursor is on |
| daw | delete the whole word your cursor is on and whitespace after it |
| p | put after cursor |
| P | put before cursor |
| xp | transpose letters (start on the first letter to switch) |
| "*yy | yank to clipboard |
| "*p | paste from clipboard |
| v | visual mode |
| . | repeat last edit |
| r | replace one character |
| R | replace mode -- like entering insert mode but with overwrite on, except backspace undoes a change instead of deletes |
| d<movement> | delete according to the movement command that follows |
| c<movement> | just like delete, but leaves you in insert mode afterwards |
| x | delete letter, same as dl |
| X | delete letter to the left of the cursor, same as dh |
| D | delete to the end of the line, like d$ |
| C |  c$  (change to end of the line) |
| s | cl  (change one character) |
| S | cc  (change a whole line) |


