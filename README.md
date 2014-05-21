About this fork
===============

This is a stripped version of CyberShadow's ae graphics module introduced here:
http://blog.thecybershadow.net/2014/03/21/functional-image-processing-in-d/

I wanted this graphics package to be easily available through DUB to build upon it.

**For better or worse**, this fork happened because modifying ae to be used as a DUB package was deemed difficult.

Find everything about the whole ae library here: https://github.com/CyberShadow/ae
If you prefer managing D projects with git submodules, it will be easier to use the original library.

What was removed:
- Everything unrelated to the graphics package.
- SDL image import to avoid a Derelict dependency (TODO re-enable this through optional DUB dependencies).
- GDI+ module which is Win32-specific (like-wise it could be included back, but Win32 bindings are not DUBified).

License
=======

This library is licensed under the [Mozilla Public License, v. 2.0](http://mozilla.org/MPL/2.0/).
Some modules may have a different license (e.g. public domain); check the comments at the top of each module for details.
You can generally expect the library to be GPL-compatible.

Warning
=======

This fork is maintained by hand. It will inevitably diverge from the ae library, so I will merge back changes here. All files are identical except the 2 added `package.d`.
