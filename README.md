texnotes
--------

In order to compile this document, you will need a LaTeX distribution. I use
texlive, so that's the best supported. On Arch Linux, this is provided by
the package texlive-most. Other Linux distros will require different setups.

If any packages are not included when you attempt to compile, they should be
available at CTAN. I don't use anything too obscure in this document.

To compile, run these commands in order:

    pdflatex notes.tex
    biblatex notes
    makeindex notes
    pdflatex notes.tex
    pdflatex notes.tex

in the root folder. In order to get figure labels and related things working
properly, you'll probably need to run this three times.

All figures should be included by default. Also, since I use natbib instead
of some of the nicer bibliography managers like biblatex, there is no need to
run a separate bibliography builder when compiling. It should all happen
automatically.
