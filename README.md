# gnumake-windows
Instructions for building [Gnu Make](https://www.gnu.org/software/make) as a native windows application

All patches under the same license as sources of [Gnu Make](https://www.gnu.org/software/make): [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) or later

Author of the patches: Michael M. Builov (mbuilov@gmail.com)

# Fixed Windows-specific bugs:
 - detect too small or empty source Makefile
 - don't hang on Ctrl-C

# Other fixes:
 - fix for inconsistency with fake function arguments, see http://savannah.gnu.org/bugs/?49841
 - ability to enable/disable warnings about use of undefined numeric variables (function arguments)
 - optimizations for Gnu Make functions: expand, sort, filter, error
 - support for ANSI color escape sequences in Windows console
 - build fix for old Visual Studios

# Instructions for building native gnumake.exe for Windows:
  [`make-4.3-build.txt`](/make-4.3-build.txt)

## Pre-built executables:
- [`gnumake-4.3.exe`](/gnumake-4.3.exe) - gnu make 4.3 built for windowsXP/x86
- [`gnumake-4.3-x64.exe`](/gnumake-4.3-x64.exe) - gnu make 4.3 built for windows7/x64

## Variants for makefile writers

1) added warnings about use of environment variables
2) extra warnings about use of undefined variables
3) run with implicitly added -rR --warn-undefined-variables switches

- [`gnumake-4.3-dev.exe`](/gnumake-4.3-dev.exe) - gnu make 4.3 built for windowsXP/x86 (development version)
- [`gnumake-4.3-dev-x64.exe`](/gnumake-4.3-dev-x64.exe) - gnu make 4.3 built for windows7/x64 (development version)
