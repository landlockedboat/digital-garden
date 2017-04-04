lun abr  3 13:19:19 CEST 2017


^ This is done with `:read !date`, btw.

* `.`: repeats the previous change. Think about it as a reverse `u`.
* `f{char}`: finds the next character `char` and moves the cursor to it.
* `;`: repeats the previous search. Think about it as a `.` for finding.
`,` is the reverse. 
* `*`: searches for the word under the cursor.

The dot formula: One keystroke to move, one keystroke to execute.

Moving around in insert mode is analogous to eviting Insert mode, pressing
the according hjkl key and diving back into Insert mode. Disgusting.

* `daw`: `delete-a-word`. `aw` is not a motion, rather a text object. `daw` 
works even if our cursor is at the end of the word.

* `<C-a>`: Adds the {count} to the number the cursor is in. `<C-x>` substracts.
If no number is found in the cursor, vim jumps to the nearest one in the line.

## Insert mode

* `<C-h>`: delete back one character
* `<C-w>`: delete back one word
* `<C-u>`: delete till start of line
* `<C-o>`: enter insert normal mode
* `<C-r>{register}`: yank text in current position. If we use the expression
operator `=` we can yank simple VimScript arithmetic.
* `<C-v>`: insert an arbitrary character either by its number or by a 
keystroke. This is useful for inserting tab characters `<C-v><Tab>` when 
indenting with spaces.



