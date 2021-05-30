# HarvardAGPS
A simple solution for Harvard AGPS bibliography style for LaTeX/BiBTeX use.

This file was created using makebst, then modified.
To use this style, copy the following into the TeX document prior to \begin{document} and make sure to have the .bst file in the working directory.

\usepackage{natbib}
\usepackage[hyphens]{url}
\usepackage[pdftex,bookmarksnumbered,hidelinks,breaklinks]{hyperref}
\bibliographystyle{agps}
\setcitestyle{aysep={}}

The regular \cite{} rules apply here.
I have made a function in the bibliography for "@online", where the note acts as a "viewed" field.
i.e. 
    @online{someauthor2021,
    author = {Some Guy},
    title = {Some Online Source},
    year = {2021},
    url = {<https://www.someonlinepublisher.com>},
    note = {Viewed 25 August 2020},
    }


This should cater to the Harvard AGPS style needs (more or less, will address bugs and needs as they arise).
