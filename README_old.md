# Express-Beamer

Yet another Beamer theme !
Please tell me if you have any request, advice, etc...!!!

[/slide.pdf](/slide.pdf) is the output pdf.

![slide image](/doc/slide-4up.png)


## Getting started
### Prerequisites
- latexmk

### Installation
```bash
git clone https://github.com/sano-jin/express-beamer.git`
make
```

### Usage

The following code shows a minimal example of a Beamer presentation.

```tex
\documentclass[xetex, unicode, 10pt]{beamer}
\usepackage{sty/style} 
\title{A minimal example}
\date{\today}
\author{Author}
\institute{Institute}
\begin{document}
  \maketitle
  \section{First Section}
  \begin{frame}{First Frame}
    Hello, world!
  \end{frame}
\end{document}
```

Take a look at [/tex/slide.tex](/tex/slide.tex) and edit this.

The output [/slide.pdf](/slide.pdf) is quite self explanatory (or at least, designed to be).
Please take a look at it!

### Customization

Customization is fairly easy.

for example, if you want to change the color schemes, you can just overwrite the default color theme like the following:

```tex
\definecolor{backgroundcolor}{RGB}{50, 50, 50}
\definecolor{textcolor}{RGB}{235, 235, 235}
\definecolor{maincolor}{RGB}{255, 241, 118}
\definecolor{accentcolor}{RGB}{70, 164, 199}
```

Then you can get the following slide. Beautiful!

![slide image](/doc/dark-theme-slide-4up.png)

## Contact

Feel free to contact me at [twitter@sano65747676](https://twitter.com/sano65747676).

## Todos

- [ ] Translate Japanese in the slide to English.
- [ ] Provide the way to merge files into one `sty` file.


## Directory Structure
```
+ tex/             # A directory for "tex" files.
|  + slide.tex     # What you need to edit.
|
+ fig/             # A directory for some figures and source codes.
|  + sample.tex    # A sample source code.
|  + logo.png      # Your Logo! Please replace it with your own!
|
+ sty/             # A directory for "sty"ling files.
|  |
|  + style.sty     # The main file for styling.
|  + source.sty    # For syntax highlighting LMNtal source codes.
|  + japanese.sty  # For some Japanese settings.
|  + jlisting.sty  # For source codes using Japanese.
|  + citation      # For the custom "footcite".
|
+ theme/           # Adirectory for our custom theme.
|  + ...           # Some styling files.
|
+ ref.bib          # For citing the references.
+ Makefile
+ latexmkrc
+ slide.pdf        # Output slide!
```




