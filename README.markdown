# Description
This is a LaTeX template meeting the submission requirements
for the 2014 ICIS Doctoral Consortium.

## Requirements
* Document MUST be compiled with XeLaTeX because I'm not sure how else to change
  the default font. Should be too much of a problem.

## Use
Set `\documentclass{icisdoc}` and put `icisdoc.cls` and `misq.bst` in the directory with
your main LaTeX document. In order to fill the template, you need to set a few
options in your TeX file. These are demonstrated in `testdocconsort.tex`.

```latex
\shorttitle{}     % Give this document a short title (8 words or fewer)
```
At the end of your document, put the following to place your references section
and use the `misq.bst` file.

```latex
\bibliographystyle{misq}
\bibliography{references}
```

## Recommendations

In addition to the usage requirements above, I have a few recommendations to
make using this as simple as possible.

1. Use Natbib for in-text citations. It lets you do nice things with citations
   in an easily understandable way. While I believe the `misq.bst` file will
   work for biblatex, I've only tested with Natbib.
2. If you use Natbib, put this in your document head to conform with MISQ style,
   as in the example LaTeX document:

```latex
\usepackage[authoryear,sort]{natbib}

\setcitestyle{aysep={}}
```
