### Movement

| command | description |
| ------- | ----------- |
| control-f | page down |
| control-b | page up |
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


