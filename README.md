# svgtopdfvialatex
A small script to automatise handling of latex-commands in svgs. Exports pdf, pdf_tex and both combined using Inkscape.

Scope
-
Automatic processing of svg-vector graphics for usage in pdflatex and friends. Input is a  *.svg file, output are two pdf files (one containing only the image information and one containing  the image information as well as the latex processed text-information) and a pdf_tex file with commands to be input into a tex document. Usually one would to  `\input{}` the pdf_tex into a tex file and ignore the combined pdf, but there might be some circumstances where a standalone pdf is needed (say for isolated viewing)


Prerequisites
-
bash, a sufficently new version of inkscape, pdflatex

Usage
-
`svgtopdfvialatex file.svg` (handles multiple input files as well)

Warning
-
Comes with absolutely no guarantee. There is a `rm -f *` inside that is not well protected, beware. 
