# Generic template in Org-mode for the first submission of an academic manuscript as a PDF

This is an org-mode variant of the main.tex file in the MooersLab/manuscriptInLaTeX [repo](https://github.com/MooersLab/manuscriptInLaTeX).
This template is for people who must write research papers in org.
The support for writing in LaTeX in Emacs is also excellent.


## Installation

1. Git clone the repo.
2. Copy main.org to a your project folder.
3. Load main.org file in Emacs via the File pulldown or `C-x C-f`.
4. Edit the file to customize to your manuscript.
5. Edit the path to your global.bib file.
5. Enter `C-c C-e l o` to compile and open the resulting PDF in your default PDF viewer.

It takes several seconds on a 2018 MacBook Pro with 32 GB of RAM. 
There is a better way. 
The correpsonding LaTeX compiles faster in Overleaf, which also provides superior support for collaborative editing by non-LaTeX using colleagues.
Sadly, Overleaf does not read org files.

## Postscript Oct 10, 2022
My approach was developed independently of another [[https://github.com/fangohr/template-latex-paper-from-orgmode/issues/4][solution]] found here. 

## Related sites

