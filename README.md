http://vimdoc.sourceforge.net/

### Movement

| command | description |
| ------- | ----------- |
| control-f | page down |
| control-b | page up |
| control-u | half page down |
| control-d | half page up |
| e, w, E, W | forward by a word |
| b, B | backwards by a word |
| f\<char\>, t\<char\> | search forward to the next occurrence of char on this line |
| F\<char\>, T\<char\> | search backwards to the previous occurrence of char on this line |
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
| \`< \`>| go to the beginning or end of the visual area |
<!-- ` -->

### Search
| command | description |
| ------- | ----------- |
| / | search |
| ? | search backwards |

### Buffers
| command | description |
| ------- | ----------- |
| :e \<filename\> | open file |
| :r \<filename\> | insert file |
| set wildmenu and wildmode=longest:list | better tab completion in commands |
| :ls or :buffers | list buffers |
| :bd | close buffer without quitting vim |
| :bn | next buffer |
| :bp | previous buffer |
| :tabe | open file in a new tab |
| :tab split | add a new tab with this file |
| gt | move between tabs |

### Splitting the window
| command | description |
| ------- | ----------- |
| :split | split horizontally |
| :vsp or :vsplit | split vertically |
| control-w w | move to the other window |
| control-w \<arrow key or hjkl\> | move to window in that direction |
| control-w o or :only | close other windows |
| control-w + | increase window size |
| control-w + | decrease window size |
| control-w \<HJKL\> | move the window in that direction |

### Registers and Macros
| command | description |
| ------- | ----------- |
| . | repeat last edit |
| "[a-z]y | yank to register |
| "[a-z]d | delete to register |
| "[a-z]p | put from register |
| "*yy | yank to clipboard |
| "*dd | delete to clipboard |
| "*p | paste from clipboard |
| q[a-z] | start recording macro -- : commands are recorded too |
| q | stop recording macro |
| @[a-z] | playback macro |
| @@ | playback last played macro |
| q[A-Z] | start appending to macro |

Recording a macro to a register is exactly the same as copying text to that register where the text are vim commands.  So another way to record a macro is simply to type out the commands, then copy them to a register.  Or, if you want to edit a macro, you can paste the register to see the commands, make changes, then copy the commands again.  

### Substitute
| command | description |
| ------- | ----------- |
| :s/orig/new/ | replace the first occurrence of orig with new on this line |
| :%s/orig/new/ | replace the first occurrence of orig with new on all lines |
| :%s/orig/new/g | replace all occurrences of orig with new on all lines |
| :%s/orig/new/gc | replace all occurrences of orig with new on all lines, but ask for confirmation for each |
| :patt1[,patt2]s/orig/new/g | replace all occurrences of orig with new in the given range. |

The range patterns could be:
 - . for the current line
 - 1 for the first line
 - any number for that line number
 - $ for the last line
 - /pattern/ the next line that contains the pattern
 - ?pattern? the previous line that contains the pattern
 - range-N or range+N to get to N lines before or after the range.
 - 'mark


For example, to make a change betweeen lines matching a pattern:
:?pattern?,/pattern/s=orig=new=g

Similarly, the "global" command executes a command on every matching line:
	:[range]g/{pattern}/{command}

### Visual mode
| command | description |
| ------- | ----------- |
| v | visual mode (select a region) |
| V | visual mode working on lines |
| control-v | select a rectangle |

While a rectangle is selected:

| command | description |
| ------- | ----------- |
| I\<text\>\<Esc\> | add \<text\> to each line (to the left of the visual block}.  Note that while typing the text, it will only appear on the first line, but after \<Esc\>, it will appear on all lines.  Short lines which aren't touched by the rectangle will be unaffected. |
| $ | When selecting a rectangle: extend the rectangle to the end of each line |
| A\<text\>\<Esc\> | add <text> to each line (to the right of the visual block}.  Short lines WILL be changed |
| c\<text\>\<Esc\> | Replace existing rectangle with the new text on each line.  Skip short lines. |
| C\<text\>\<Esc\> | Replace existing rectangle with each line extended to the end of the line with the new text on each line.  Skip short lines. |
| U | make uppercase |
| u | make lowercase |
| ~ | swap case |
| r\<char\> | replace with a single character (as many repetitions of that character as necessary) |
| J | join lines |
| > | replace with a single letter (as many repetitions of that letter as necessary) |
| < | Decrease indent |
| > | Increase indent |
| = | reindent |

### Other

| command | description |
| ------- | ----------- |
| u | undo |
| control-r | redo |
| set expandtab tabstop=4 shiftwidth=4 | set tab size |
| gg=G | reindent the whole file |
| :so ~/.vimrc | reload .vimrc file |
| :set incsearch hlsearch | turn on incremental search and highlight search |
| diw | delete the whole word your cursor is on |
| daw | delete the whole word your cursor is on and whitespace after it |
| xp | transpose letters (start on the first letter to switch) |
| p | put after cursor |
| P | put before cursor |
| r | replace one character |
| R | replace mode -- like entering insert mode but with overwrite on, except backspace undoes a change instead of deletes |
| d\<movement\> | delete according to the movement command that follows |
| c\<movement\> | just like delete, but leaves you in insert mode afterwards |
| x | delete letter, same as dl |
| X | delete letter to the left of the cursor, same as dh |
| D | delete to the end of the line, like d$ |
| C |  c$  (change to end of the line) |
| s | cl  (change one character) |
| S | cc  (change a whole line) |
| set unmodifiable | read-only mode |
| :saveas \<filename\> | save to a different file |
| gUw | uppercase next word |
| guw | lowercase next word |




