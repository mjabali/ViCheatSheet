####Vi Cheat Sheet
==================================

####Cursor movement

h - move left<br>
j - move down<br>
k - move up<br>
l - move right<br>
w - jump by start of words (punctuation considered words)<br>
W - jump by words (spaces separate words)<br>
e - jump to end of words (punctuation considered words)<br>
E - jump to end of words (no punctuation)<br>
b - jump backward by words (punctuation considered words)<br>
B - jump backward by words (no punctuation)<br>
0 - (zero) start of line<br>
^ - first non-blank character of line<br>
$ - end of line<br>
G - Go To command (prefix with number - 5G goes to line 5)<br>
Note: Prefix a cursor movement command with a number to repeat it. For example, 4j moves down 4 lines.<br>

####Insert Mode - Inserting/Appending text

i - start insert mode at cursor
I - insert at the beginning of the line
a - append after the cursor
A - append at the end of the line
o - open (append) blank line below current line (no need to press return)
O - open blank line above current line
ea - append at end of word
Esc - exit insert mode

*Editing

r - replace a single character (does not use insert mode)
J - join line below to the current one
cc - change (replace) an entire line
cw - change (replace) to the end of word
c$ - change (replace) to the end of line
s - delete character at cursor and subsitute text
S - delete line at cursor and substitute text (same as cc)
xp - transpose two letters (delete and paste, technically)
u - undo
. - repeat last command

*Cut and Paste

yy - yank (copy) a line
2yy - yank 2 lines
yw - yank word
y$ - yank to end of line
p - put (paste) the clipboard after cursor
P - put (paste) before cursor
dd - delete (cut) a line
dw - delete (cut) the current word
x - delete (cut) current character

*Exiting

:w - write (save) the file, but don't exit
:wq - write (save) and quit
:q - quit (fails if anything has changed)
:q! - quit and throw away changes

*Search/Replace

/pattern - search for pattern
?pattern - search backward for pattern
n - repeat search in same direction
N - repeat search in opposite direction
:%s/old/new/g - replace all old with new throughout file
:%s/old/new/gc - replace all old with new throughout file with confirmations

*Working with multiple files

:e filename - Edit a file in a new buffer
:bnext (or :bn) - go to next buffer
:bprev (of :bp) - go to previous buffer
:bd - delete a buffer (close a file)
:sp filename - Open a file in a new buffer and split window
ctrl+ws - Split windows
ctrl+ww - switch between windows
ctrl+wq - Quit a window
ctrl+wv - Split windows vertically
