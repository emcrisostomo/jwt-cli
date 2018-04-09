[![License](https://img.shields.io/badge/license-GPL--3.0-blue.svg?style=flat)](https://github.com/emcrisostomo/jwt-cli/blob/master/LICENSE)

jwt-cli
=======

`jwt-cli` is a shell library to decode JWT tokens.

Prerequisites
-------------

`jwt-cli` requires the following programs to be present on the `${PATH}`:

  * `jq`
  * `openssl`
  * `zsh`

Getting jwt-cli
---------------

A user who whishes to build this package should get a [release
tarball][release].  A release tarball contains everything a user needs to build
the package on his system, following the instructions detailed in the
Installation section below and the `INSTALL` file.

A developer who wishes to modify this package should get the sources (either
from a source tarball or cloning the repository) and have the GNU Build System
installed on his machine.  Please read `README.gnu-build-system` to get further
details about how to bootstrap this package from sources on your machine.

Getting a copy of the source repository is not recommended unless you are a
developer, you have the GNU Build System installed on your machine, and you know
how to bootstrap it on the sources.

[release]: https://github.com/emcrisostomo/jwt-cli/releases

Installation
------------

See the `INSTALL` file for detailed information about how to configure and
install this package.

Usage
-----

The following operation decodes a JWT token:

    $ jwt-decode token

Bug Reports
-----------

Bug reports can be sent directly to the authors.

-----

Copyright (c) 2018 Enrico M. Crisostomo

This program is free software; you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation; either version 3, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see <http://www.gnu.org/licenses/>.
