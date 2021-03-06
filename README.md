# musictheory.net changes

This is a fork of the last public release (1.8) of [Loris](http://cerlsoundgroup.org/Loris/)
with select changes for Python 3 compatibility.

## Installation on macOS

```
git clone https://github.com/musictheory/loris.git
cd loris
export PYTHON=/Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7
./configure --exec_prefix=/Library/Frameworks/Python.framework/Versions/3.7 CPPFLAGS=-I/Library/Frameworks/Python.framework/Versions/3.7/include/python3.7m
make
sudo make install
```

# Original README

## Welcome to Loris.

Loris is an open source C++ class library implementing analysis,
manipulation, and synthesis of digitized sounds using the Reassigned
Bandwidth-Enhanced Additive Sound Model.

For more information about Loris and the Reassigned Bandwidth-Enhanced
Additive Model, contact the developers at loris@cersloundgroup.org, or
visit them at http://www.cerlsoundgroup.org/Loris/.

The primary distribution point for Loris is SourceForge
(http://loris.sourceforge.net) and its mirrors.

Loris is free software. Please see the file COPYING for details.

For documentation, please see the files in the doc subdirectory.

For a list of major changes to Loris, organized by release number,
please see the file NEWS.

## INSTALLATION: 

For generic configuration and installation instructions, see
the file INSTALL.

In order to compile and link the Loris library and scripting extensions,
you will need a modern, reasonably standard-compliant C++ compiler (and
linker, etc.). To build scripting extensions, such as the Python module,
you will also need SWIG, a tool that connects programs written in C and
C++ with a variety of high-level programming languages, available at
www.swig.org 

For best performance, you should also install the FFTW Fourier transform
library, available at www.fftw.org. Mac OS X users see note below. FFTW
is covered by its own license and copyright, and is entirely separate
from Loris. FFTW is not required to build or use Loris.


## MacOS INSTALLATION:

Loris can be built using the standard GNU tools from a Terminal window
under Mac OS X (Darwin), follow the instructions for the standard
distribution. You will, of course, need the developers' tools, available
from Apple, in order to compile Loris (or anything else) under OS X. It
is also possible to build Loris using Xcode under OS X.

NOTE: By default, FFTW builds and installs only static libraries under
Mac OS X. Loris needs to link against the dynamic FFTW library. You need
to explicitly enable dynamic linking when building FFTW so that the
dynamic (shared) library is built.


## COPYRIGHT AND LICENSE:

Loris is Copyright (c) 1999-2010 by Kelly Fitz and Lippold Haken

Loris is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY, without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
file COPYING or the GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

loris@cerlsoundgroup.org
http://www.cerlsoundgroup.org/Loris/
