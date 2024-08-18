![Version](https://img.shields.io/static/v1?label=manuscriptInOrg&message=0.2&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Manuscript template in org for the first submission 

The first submission of a research paper for peer review can be in a generic format as a PDF.
It is silly to submit the manuscript as if it were a galley proof at this stage.
The advantage of a plain generic template is that it can be submitted to many different journals.

This is an org-mode variant of the main.tex file in the MooersLab/manuscriptInLaTeX [repo](https://github.com/MooersLab/manuscriptInLaTeX).
This template is for people who prefer to write research papers in org.
The support for writing in LaTeX in Emacs is also excellent.

## Edit on-line in your favorite text editor
### Editing via GhostTex on Overleaf
You can edit LaTeX documents stored on Overleaf inside Emacs or a half dozen other text editors via GhostText.
See slides here [here](https://github.com/MooersLab/DSW22ghosttext) and video [here](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d).
Note that I configured the Emacs Atomic package to open files from Overleaf in the LaTeX mode.
This brings the full power of Emacs to Overleaf.
Compiling tex files in Overleaf is faster.

### Editing via GhostTex on GitHub
An alternative approach to collaborative editing is to do the editing on a private Github repo.
GhostText enables text editing in the text area when in the edit mode on Github. 
Configure Atomic to cause Emacs to open org files from Github in org mode.
This approach assumes that all of the collaborators are using Emacs to do their editing.
Non-Emacs users could just use the editing tools in GitHub to edit the file directly, or you might be able to configure their editors to open org files via GhostText.

## Installation

1. Git clone the repo `git clone https://github.com/MooersLab/manuscriptInOrg.git`.
2. Copy main.org to a your project folder.
3. Load main.org file in Emacs via the File pulldown menu or `C-x C-f`.
4. Edit the file to customize to your manuscript.
5. Edit the paths to your global.bib file and your image files.
6. Enter `C-c C-e l o` to compile and open the resulting PDF in your default PDF viewer.

Compiling takes several seconds on a 2018 MacBook Pro with 32 GB of RAM. 
There is a better way. 
The corresponding LaTeX compiles faster in Overleaf, providing superior support for collaborative editing by non-LaTeX using colleagues.
The latter is a deficiency in Emacs that some of working hard to address.
Sadly, Overleaf does not read org files.

## Assumptions

1. LaTeX is installed with all of the required style files. However, my installation was missing the **break cities.sty** file. I installed this with the ``sudo port install texlive-bibtex-extra`` command.
2. Emacs is using used to edit the org file.
3. You will use the LaTeX cite command and let LaTeX handle the generation of the literature cited section. This is the citar and so on can help with finding the right citekey.

## Postscript Oct 10, 2022
My approach was developed independently of another [solution](https://github.com/fangohr/template-latex-paper-from-orgmode/issues/4) found here. 

## Postscript May 16, 2023
I had upgraded my operating system to Ventura, but I had not properly migrated my MacPorts. I found that I was missing the breakcities.sty file.

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

Note that [latex-emacs profile](https://github.com/MooersLab/latex-emacs) has functions for converting LaTex lists into org-markdown lists.


## Update history

|Version      | Changes                                                                                                                                    | Date                 |
|:-----------:|:------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|
| Version 0.2 |   Added badges, funding, and update table.                                                                                                 | 2024 May 21          |


## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)

