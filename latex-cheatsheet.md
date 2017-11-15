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

Enumerate Labels
----------------
    \documentclass{article}
    \usepackage{enumitem}
    \begin{document}

    \begin{enumerate}[label=(\alph*)]
    \item an apple
    \item a banana
    \item a carrot
    \item a durian
    \end{enumerate}

    \begin{enumerate}[label=(\Alph*)]
    \item an apple
    \item a banana
    \item a carrot
    \item a durian
    \end{enumerate}

    \begin{enumerate}[label=(\roman*)]
    \item an apple
    \item a banana
    \item a carrot
    \item a durian
    \end{enumerate}

    \end{document}
