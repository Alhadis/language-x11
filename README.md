<!-- vim:se noet lbr tw=72 sts=0 sw=4 ts=4 wrap:
--*- fill-column: 72; truncate-lines: nil; word-wrap: t; -*-->

X11/X.org config syntax highlighting support
========================================================================

This package adds syntax highlighting for a plethora of X11-related file
formats (specified by [FreeDesktop.org][1]). Currently, this includes:

* [x] `.Xresources` / `.Xdefaults`
* [ ] `xorg.conf.d/*.conf`
* [ ] XSM startup applications lists: `.xsmstartup`, `system.xsm`
* [ ] Colour name databases: `rgb.txt`

Notice of future breaking changes
------------------------------------------------------------------------
Eventually, this will also include two grammars currently provided by an
existing package ([`language-fontforge`][2]). This will involve breaking
changes for any third-party code that references the following grammars:

* [ ] [`source.fontdir`](https://bit.ly/3WlgBkq)
* [ ] [`source.xlfd`](https://bit.ly/3KD7jO8)

The rationale for the migration is that both formats, while font-related
in one sense, are much more closely-related to the X11 system. Backwards
compatibility will be attempted by listing this package as a dependency,
although with the demise of the Atom project, no package registries will
be updated to reflect [`language-fontforge`][2]'s next tagged release.


<!-- Referenced Links ------------------------------------------------->
[1]: https://www.freedesktop.org/wiki/Specifications/
[2]: https://github.com/Alhadis/language-fontforge
