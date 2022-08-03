# `spath3` TikZ library

This is a library for manipulating TikZ's _soft paths_.  When TikZ reads a
path construction, it first constructs a _soft path_ before converting it into
an actual path in the output document.  A _soft path_ contains the information
needed to build the path in a TeX macro, whence it can be manipulated before
it is _baked_.

This library provides ways of modifying these paths before they are baked.

It also provides some sub-packages which make use of this facility:

1. `knots` for drawing knot diagrams, sorting out the crossings at
   intersections
2. `calligraphy` which turns a path into one that might be drawn by a
   calligraphic pen
3. `spath3` which is a user-level interface to the core functionality

# Installation

These libraries are on [CTAN](https://ctan.org/pkg/spath3?lang=en) and are
included in TeXLive and MikTeX.  You should obtain them from one of those
sources.  If you know that you need the most up to date version from here,
then download the file `spath3_code.dtx` and run `tex spath3_code.dtx` to generate the
files.

# Documentation

The simplest way to get the documentation is via `texdoc` or from [CTAN](https://ctan.org/pkg/spath3?lang=en).  To generate it from source, run `pdflatex` on one of the `_doc.tex` files or on `spath3.tex`.
