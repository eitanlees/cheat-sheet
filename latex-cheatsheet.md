Latex Cheatsheet
================

General Notes
-------------
You should also be using \(...\) instead of $...$ too

Margins
-------
\usepackage[margin=0.5in]{geometry}

Spacing
-------
\usepackage{setspace}
\doublespacing

Biber
-----

A possible bib fix --> rm -rf `biber --cache`

Numbering Signle line
---------------------

\newcommand\numberthis{\addtocounter{equation}{1}\tag{\theequation}}
