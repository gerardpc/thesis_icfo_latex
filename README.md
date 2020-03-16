# Latex thesis template
LaTeX template for PhD theses (or similar document format), based on the memoir document type.

The repository is divided in 5 folders:

0 Thesis manuscript
-----------
Has the main file "thesis.tex", which includes via \include all the other text. This is the .tex file that needs to be compiled to create the thesis pdf. To ensure that the links and references are updated, run each time
> pdflatex + bibtex + pdflatex + pdflatex.

1 Text contents
-----------
Contains the .tex files that are included in "thesis.tex". These files are:

- "title.tex", contains the titleplage.
- "abstract.tex", contains the thesis abstract.
- "acknowledgements.tex", contains the acknowledgments.
- "main_chapters.tex", contains the text of the thesis chapters.
- "publications.tex", contains a page with the publications of the thesis.
- "annexes.tex", contains the annexes, in the same format as in the chapters.
- "references.bib", contains the references cited in the text in bibtex style.

2 Figures
-----------
Contains the figures included in the text, separated by folders (for cleanliness).

3 Packages and template
-----------
Contains:

- "def_shortcuts.tex", a tex file with my own math style definitions and environments (and potentially more).
- "memoir_template.tex", the actual template of the thesis. Edit this file to change the margins, looks, chapter style, etc.
- "packages.tex" has the latex packages of the "thesis.tex" document.

4 Print subpdf
-----------
Although it is not really necessary, it is convenient to have a "select_pages.tex" file that prints a subpdf (i.e., only a few pages) of the file "thesis.pdf". This way you can send to your supervisor only a few pages of the thesis for revision (for instance a single chapter).
