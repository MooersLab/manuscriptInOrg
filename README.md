# Manuscript template in org for the first submission 

The first submission of a research paper for peer review can be in a generic format as a PDF.
It is silly to submit the manuscript as if it were a galley proof at this stage.
The advantage of a plain generic template is that it can be submitted to many different journals.

This is an org-mode variant of the main.tex file in the MooersLab/manuscriptInLaTeX [repo](https://github.com/MooersLab/manuscriptInLaTeX).
This template is for people who prefer to write research papers in org.
The support for writing in LaTeX in Emacs is also excellent.

You can edit LaTeX documents stored on Overleaf inside Emacs via GhostText.
See slides here [here](https://github.com/MooersLab/DSW22ghosttext) and video [here](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d).
This brings the full power of Emacs to Overleaf.
Compiling tex files in Overleaf is faster.

An alternative approach to collaborative editing would be to do the editing on a private Github repo.
GhostText enables the 

## Installation

1. Git clone the repo `git clone https://github.com/MooersLab/manuscriptInOrg.git`.
2. Copy main.org to a your project folder.
3. Load main.org file in Emacs via the File pulldown menu or `C-x C-f`.
4. Edit the file to customize to your manuscript.
5. Edit the paths to your global.bib file and your image files.
6. Enter `C-c C-e l o` to compile and open the resulting PDF in your default PDF viewer.

Compiling takes several seconds on a 2018 MacBook Pro with 32 GB of RAM. 
There is a better way. 
The correpsonding LaTeX compiles faster in Overleaf, which also provides superior support for collaborative editing by non-LaTeX using colleagues.
The latter is a deficiency in Emacs that some of working hard to address.
Sadly, Overleaf does not read org files.

## Assumptions

1. LaTeX is installed with all of the required style files. I found my installation to be missing the **breakcites.sty** file. I installed this with the ``sudo port install texlive-bibtex-extra`` command.
2. Emacs is using used to edit the org file.

## Postscript Oct 10, 2022
My approach was developed independently of another [solution](https://github.com/fangohr/template-latex-paper-from-orgmode/issues/4) found here. 

## Postscript May 16, 2023
I had upgraded my operating system to Ventura. I had not migrated my macports properly. I found that I was missing the breakcites.sty file.

## Related sites

- [Writing log template in Org-mode](https://github.com/MooersLab/writingLogTemplateInOrg)
- [Writing log template in LaTeX](https://github.com/MooersLab/writingLogTemplate)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX/edit/main/README.md)
- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg/edit/main/README.md)
- [Workbook for 2022 for tracking time spent and words written by project](https://github.com/MooersLab/writingProgress2022)
- [Slideshow template in LaTeX](https://github.com/MooersLab/slideshowTemplateLaTeX)
- [Annotated bibliography Template in LaTeX](https://github.com/MooersLab/annotatedBibliography)
- [Diary for 2022 in LaTeX](https://github.com/MooersLab/diary2022inLaTeX)
- [Diary for 2023 in LaTeX](https://github.com/MooersLab/diary2023inLaTeX)
- [latex-emacs profile](https://github.com/MooersLab/latex-emacs)
- [default Emacs profile](https://github.com/MooersLab/configorg)
- [snippets for latex-mode in Emacs](https://github.com/MooersLab/snippet-latex-mode)
- [Quizzes about Emacs to improve recall of keybindings](https://github.com/MooersLab/qemacs)
- [Slides from talk about GhostText, Data Science Workshop, July 2022](https://github.com/MooersLab/DSW22ghosttext)
- [Video link to talk about GhostText, Data Science Workshop, July 2022](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d)
- [The writer's law](https://github.com/MooersLab/thewriterslaw)

Note that [latex-emacs profile](https://github.com/MooersLab/latex-emacs) has fuctions for converting LaTex lists into org-markdown lists.
