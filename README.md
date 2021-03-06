# vim-cheatsheet
My Personal VIM Cheatsheet

## Mode
Normal mode - navigate the structure of the file

Insert mode - editing the file

Visual mode - highlight portions of the file to manipulate at once

Ex mode - command mode

## Window Scroll
ctrl + e = scroll window down

ctrl + y = scroll window up

## Page Scroll
ctrl + f = scroll down one page

ctrl + b = scroll up one page

## Window Move
shift + h = move cursor to the top of the window

shift + m = move cursor to the middle of the window

shift + l = move cursor to the bottom of the window

## File Move
gg = go to top of file

shift + g = go to bottom of file

## Text Objects
w = words

s = sentences

p = paragraphs

t = tags (available in XML/HTML files)

## Motions
a = all

i = in

t = till

f = find forward

F = find backward

## Commands
d = delete

c = change(delete, then place in insert mode)

y = yank (copy)

p = paste

v = visually select

## Combinations in Text Object and Motions
w = move on  the first character of the word

e = move on the end character of the word

diw = delete in word

di[ = delete in brackets

di(space) = delete in space

caw = change all word

yi) = yank in parentheses

vaw = select all word

va" = select all "

## Additional Commands

dd / yy - delete/yank the current line

D / C - delete/change until end of line

^ / $ - move to the beginning/end of line

I / A - move to the beginning/end of line and insert

o / O - insert new line above/below current line and insert

## Repetition
. = repetition command

repeat ci' in some line with ''

Example:

Change foo with bar

Line 1

```
'foo' -> ci' then type bar
```

result :

```
'bar'
```

Line 2 

```
'foo' -> only type . 
```

result :

```
'bar'
```

## Surround

Pre-requisites : surround.vim and repeat.vim

Add ' or " etc to the beginning and end of word

Line 1

```
bag -> ysiw then type '
```

result :

```
'bag'
```

Line 2

```
bug -> only type . 
```

result : 

```
'bug'
```

