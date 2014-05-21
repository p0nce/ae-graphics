About this fork
===============

This is a stripped version of CyberShadow's ae graphics module (http://blog.thecybershadow.net/2014/03/21/functional-image-processing-in-d/), introduced here. I wanted this graphics package to be easily available through DUB to build upon it.

**For better or worse**, this fork happened because modifying ae to be used as a DUB package was deemed difficult (one of the main problem being that DUB is ill-suited for projects that follow a git sub-modules structure, without import/source sub-durectory. This makes source and imports paths leak).

Find everything about the whole ae library here: https://github.com/CyberShadow/ae

What was removed:
- everything not related to the graphics package
- SDL image import to avoid a Derelict dependencies(TODO re-enable this through optional DUB dependencies)
- GDI+ module which is Win32-specific (but likewise it could be included)

License
=======

This library is licensed under the [Mozilla Public License, v. 2.0](http://mozilla.org/MPL/2.0/).
Some modules may have a different license (e.g. public domain); check the comments at the top of each module for details.
You can generally expect the library to be GPL-compatible.

Warning
=======

This fork is maintained by hand. It shouldn't diverge from the ae library, and should follow CyberShadow's choices in ae.
