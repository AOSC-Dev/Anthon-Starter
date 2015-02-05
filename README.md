# Anthon-Starter 0.2.0 [![Travis-CI Build Status](https://travis-ci.org/AOSC-Dev/Anthon-Starter.svg?branch=0.2.0-devel)](https://travis-ci.org/AOSC-Dev/Anthon-Starter) [![https://scan.coverity.com/projects/2952](https://scan.coverity.com/projects/2952/badge.svg)](https://scan.coverity.com/projects/2952)

Installation helper for AOSC OSes, written with C.

Homepage:[https://portal.anthonos.org/ast](https://portal.anthonos.org/ast)

## License

Anthon-Starter is published under GNU GPLv2 or later.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

## Build

To build Anthon-Starter, you need these tools be installed:

* In Microsoft(R) Windows(R)
    * i686-mingw-w64
    * GNU Make (of cource)
* In Linux(R)
    * binutils-mingw-w64-i686
    * gcc-mingw-w64-i686

At present we haven't prepared `configure` (autotools) yet, but we have specified these variables in `Makefile`:

````Makefile
HOST ?= i686-w64-mingw32
CC   := ${HOST}-gcc
LD   := ${HOST}-gcc
RES  := ${HOST}-windres
````

Unless knowing what you're doing, please use the pre-configured `${HOST}` variable. Mistakenly specify or empty this variable can be failed to compile.

## Developers

* Junde Yi <lmy441900@gmail.com>
* Zixing Liu <liushuyu011@gmail.com>
* Mike Manilone <crtmike@gmail.com>
* Minhui Du <duminghui@126.com>

