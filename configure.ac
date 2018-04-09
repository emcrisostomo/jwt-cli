#                                               -*- Autoconf -*-
# Copyright (C) 2018 Enrico M. Crisostomo
#
# This program is free software; you can redistribute it and/or modify it under
# the terms of the GNU General Public License as published by the Free Software
# Foundation; either version 3, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
# FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
# details.
#
# You should have received a copy of the GNU General Public License along with
# this program.  If not, see <http://www.gnu.org/licenses/>.
#
# Process this file with autoconf to produce a configure script.
#
dnl Copyright (C) 2018 Enrico M. Crisostomo
AC_PREREQ([2.69])
AC_INIT([jwt-cli], [0.1.0], [enrico.m.crisostomo@gmail.com])
AC_COPYRIGHT([2018 (C) Enrico M. Crisostomo])
AC_REVISION([$Revision: 1.0.0$])
AC_CONFIG_SRCDIR([scripts/jwt-decode.in])
AC_CONFIG_AUX_DIR([config])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([scripts/jwt-decode])
AC_CONFIG_MACRO_DIRS([m4])
AC_CONFIG_MACRO_DIR([m4])

# Initialize Automake
AM_INIT_AUTOMAKE([-Wall -Werror gnu subdir-objects])
AM_SILENT_RULES([yes])

# Checks for programs.
AC_PATH_PROG([BASE64_CMD],  [base64],  [no])
AC_PATH_PROG([JQ_CMD],      [jq],      [no])
AC_PATH_PROG([OPENSSL_CMD], [openssl], [no])
AC_PATH_PROG([ZSH_CMD],     [zsh],     [no])

AS_VAR_IF([JQ_CMD],      [no], [AC_MSG_ERROR([jq is required.])],      [])
AS_VAR_IF([ZSH_CMD],     [no], [AC_MSG_ERROR([zsh is required.])],     [])

AS_VAR_IF([BASE64_CMD],     [no],  [], [AS_VAR_SET([BASE64_ENABLED], [yes])])
AS_VAR_IF([OPENSSL_CMD],    [no],  [], [AS_VAR_SET([BASE64_ENABLED], [yes])])
AS_VAR_IF([BASE64_ENABLED], [yes], [], [AC_MSG_ERROR([Either base64 or openssl are required.])])

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_OUTPUT
