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

i - start insert mode at cursor<br>
I - insert at the beginning of the line<br>
a - append after the cursor<br>
A - append at the end of the line<br>
o - open (append) blank line below current line (no need to press return)<br>
O - open blank line above current line<br>
ea - append at end of word<br>
Esc - exit insert mode<br>

####Editing

r - replace a single character (does not use insert mode)<br>
J - join line below to the current one<br>
cc - change (replace) an entire line<br>
cw - change (replace) to the end of word<br>
c$ - change (replace) to the end of line<br>
s - delete character at cursor and subsitute text<br>
S - delete line at cursor and substitute text (same as cc)<br>
xp - transpose two letters (delete and paste, technically)<br>
u - undo<br>
. - repeat last command<br>

####Cut and Paste

yy - yank (copy) a line<br>
2yy - yank 2 lines<br>
yw - yank word<br>
y$ - yank to end of line<br>
p - put (paste) the clipboard after cursor<br>
P - put (paste) before cursor<br>
dd - delete (cut) a line<br>
dw - delete (cut) the current word<br>
x - delete (cut) current character<br>

####Exiting

:w - write (save) the file, but don't exit<br>
:wq - write (save) and quit<br>
:q - quit (fails if anything has changed)<br>
:q! - quit and throw away changes<br>

####Search/Replace

/pattern - search for pattern<br>
?pattern - search backward for pattern<br>
n - repeat search in same direction<br>
N - repeat search in opposite direction<br>
:%s/old/new/g - replace all old with new throughout file<br>
:%s/old/new/gc - replace all old with new throughout file with confirmations<br>

####Working with multiple files

:e filename - Edit a file in a new buffer<br>
:bnext (or :bn) - go to next buffer<br>
:bprev (of :bp) - go to previous buffer<br>
:bd - delete a buffer (close a file)<br>
:sp filename - Open a file in a new buffer and split window<br>
ctrl+ws - Split windows<br>
ctrl+ww - switch between windows<br>
ctrl+wq - Quit a window<br>
ctrl+wv - Split windows vertically<br>
