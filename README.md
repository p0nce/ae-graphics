[![Build Status](https://travis-ci.org/p0nce/ae-graphics.png?branch=master)](https://travis-ci.org/p0nce/ae-graphics)

About this fork
===============

This is a stripped version of CyberShadow's ae graphics module introduced here:
http://blog.thecybershadow.net/2014/03/21/functional-image-processing-in-d/

I wanted this graphics package to be easily available through DUB to build upon it.

**For better or worse**, this fork happened because modifying ae to be used as a DUB package was deemed difficult.
Now ae is available as a DUB package but is not yet separated in sub-packages.

Find everything about the whole ae library here: https://github.com/CyberShadow/ae

If you prefer managing D projects with git submodules, it will be easier to use the original library.

What was removed:
- Everything unrelated to the graphics package.
- SDL image import to avoid a Derelict dependency (TODO re-enable this through optional DUB dependencies).
- GDI+ module which is Win32-specific (like-wise it could be included back, but Win32 bindings are not DUBified).
- ImageMagick executable wrapper.

License
=======

This library is licensed under the [Mozilla Public License, v. 2.0](http://mozilla.org/MPL/2.0/).

Warning
=======

This fork is maintained by hand. It will inevitably diverge from the ae library, so I will merge back changes here. All files are identical except the 2 added `package.d`.
