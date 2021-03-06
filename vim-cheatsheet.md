Vim Cheatsheet
==============


Standard
--------

### FileType
To check file type --> :set ft?

### Splits

Switch two splits to horizontal --> <C-w>K
Switch two splits to vertical   --> <C-w>H
Switch two splits               --> <C-w><C-x>

Open file in a horizontal split  --> :sp filename
Open file in a vertical split    --> :vsp filename

increase a number --> <CR>a
decrease a number --> <CR>x

### Find and Replace
Replace 'foo' with 'bar' (whole file)        --> :%s/foo/bar/g
Replace 'foo' with 'bar' (only current line) --> :s/foo/bar/g

### Rot13
Ceaser cipher where N is 13 --> g?

### Caseswitch
Toggle case of selected text --> ~

### Number increment
To increase a number --> <C-a>
To decrease a number --> <C-x>


Surround-vim
------------

Change surrounding object --> cs')
Delete surrounding object --> ds"
Surround a whole line     --> yss)
Surround a word           --> ysiw]

Tabularize
----------

Align text with a 'char' --> :Tabularize \char

Ctrl-P
------

To activate fuzzy search --> <C-p>
To open in a split       --> <C-v> or <C-x>

Thesaurus
---------
:OnlineThesaurusCurrentWord --> <LocalLeader>K
:Thesaurus word

Merging two files linewise
--------------------------

**Merging the files**

%!paste - Y.dat 

**Replacing multiple spaces**

%s/\s\+/ /g     

**Replacing spaces with commas**

%s/\ /,/g       

**Putting a period at the end**

%s/$/./g
