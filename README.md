# `spath3` TikZ library

This is a library for manipulating TikZ's _soft paths_.  When TikZ reads a
path construction, it first constructs a _soft path_ before converting it into
an actual path in the output document.  A _soft path_ contains the information
needed to build the path in a TeX macro, whence it can be manipulated before
it is _baked_.

This library provides ways of modifying these paths before they are baked.

It also provides two sub-packages which make use of this facility:

1. `knots` for drawing knot diagrams, sorting out the crossings at
   intersections
2. `calligraphy` which turns a path into one that might be drawn by a
   calligraphic pen
