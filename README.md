---
title:  gitit-tools/README.md
author: Christian Külker
date:   2022-02-21

---

# Abstract

This document describes briefly the aim and content of __gitit-tools__.

![Github license](https://img.shields.io/github/license/ckuelker/gitit-tools.svg)
![Github issues](https://img.shields.io/github/issues/ckuelker/gitit-tools.svg?style=popout-square)
![Github code size in bytes](https://img.shields.io/github/languages/code-size/ckuelker/gitit-tools.svg)
![Git repo size](https://img.shields.io/github/repo-size/ckuelker/gitit-tools.svg)
![Last commit](https://img.shields.io/github/last-commit/ckuelker/gitit-tools.svg)

## History

| Version | Date       | Notes                                                |
| ------- | ---------- | ---------------------------------------------------- |
| 0.1.0   | 2022-02-21 | Initial release                                      |

# Introduction

The goal of __gitit-tools__ is to add command line functions to `gitit` by
providing scripts in set that can be used to manage a `gitit` instance.

[Gitit](https://github.com/jgm/gitit) is a wiki program written by John
MacFarlane in Haskell.

# Tools

## gitit-users-account-create-single

Can be used to crate a `gitit-users` file.

Executing the command `gitit-users-account-create-single` will
write the content of one account to `gitit-users` if invoked like
this:

```shell
echo "SECRET" > password.txt
gitit-users-account-create-single -u BilboBaggings \
-e b@example.org -f password.txt > gitit-users
```
Be aware this will overwrite an existing `gitit-users` file. If no
password file is given then the password will be asked.

```shell
gitit-users-account-create-single -u Frodo -e f@example.org
```

# Author

    Christian Külker <c@c8i.org>

# License And Copyright

    Copyright (C) 2022 by Christian Kuelker

    This program is free software; you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by the Free
    Software Foundation; either version 3, or (at your option) any later
    version.

    This program is distributed in the hope that it will be useful, but WITHOUT
    ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
    FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for
    more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc., 59
    Temple Place, Suite 330, Boston, MA 02111-1307 USA

# DISCLAIMER OF WARRANTY

    THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE
    LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
    OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND,
    EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE
    ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.
    SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY
    SERVICING, REPAIR OR CORRECTION.


# LIMITATION OF LIABILITY

    IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL
    ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE
    PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
    GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
    USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
    DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
    PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
    EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
    SUCH DAMAGES.

