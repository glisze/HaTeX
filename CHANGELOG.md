
# HaTeX Changelog

This is the logchange of HaTeX. It is not exhaustive.
For a full list of changes, see the commit history of the
git repository:

https://github.com/Daniel-Diaz/HaTeX/commits/master

# Changelog by versions

## From 3.16.2.0 to 3.17.0.0

* New 'array' command (NorfairKing).
* Added package options for the hyperref package related to PDF metadata (dmcclean).
* QRCode module (dmcclean).
* New math symbols (leftaroundabout).
* Added 'cases' environment (NorfairKing).
* Changed the way subscripts and superscripts work.
  See [#67](https://github.com/Daniel-Diaz/HaTeX/pull/67).
  Also [#78](https://github.com/Daniel-Diaz/HaTeX/pull/78).
* LaTeX parser is now configurable.
  Currently, only configurable option is verbatim
  environments.

## From 3.16.1.1 to 3.16.2.0

* New differentiation symbols (AMSMath).
* Fix for integralFromTo.
* Extend definitions for the Num class instance of LaTeXT.
* Show and Eq instances of LaTeXT dissappear if base version
  is greater or equal to 4.5.0.0.

## From 3.16.1.0 to 3.16.1.1

* Full compatibility without warnings with GHC-7.10.

## From 3.16.0.0 to 3.16.1.0

* Pretty-printer: Use softline instead of line after commands.
* Compatibility with GHC-7.10.
* Added accent commands to AMSMath (dmcclean).
* Missing Num and Floating class methods now have a default implementation,
  using the new `operatorname` function (dmcclean).
* Added `imath` and `jmath` to AMSMath (dmcclean).
* Support for parsec-3.1.9 (snoyberg).

Thanks to Douglas McClean (dmcclean@GitHub) for the AMSMath additions.

## From 3.15.0.0 to 3.16.0.0

* New package implemented: relsize.
    Thanks José Romildo Malaquias.
* Fixed bug in autoBrackets ([#42](https://github.com/Daniel-Diaz/HaTeX/pull/42)).

## From 3.14.0.0 to 3.15.0.0

* New package implemented: AMSSymb.
* Package beamer further developed.
* Bug fix: [#35](https://github.com/Daniel-Diaz/HaTeX/issues/35).
* Added common numeric sets to AMSSymb.
* Breaking change: AMSMath functions 'pm' and 'mp' changed their
  type from `LaTeXC l => l -> l -> l` to `LaTeXC l => l`.
* Additions to the AMSMath module.

## From 3.13.1.0 to 3.14.0.0

* Fixed link in cabal file.
* Added support for arguments delimited by parenthesis (experimental).
* More tests on parsing.
* Parser now backtracks when failing in argument parsing.

## From 3.13.0.1 to 3.13.1.0

* New function ``matrixTabular`` to create tables from matrices.
* Modified LaTeX Monoid instance to make monoid laws hold.
* Some documentation improvements.
* Added this CHANGELOG!
