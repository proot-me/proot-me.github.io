PRoot
=====

*chroot, mount --bind, and binfmt_misc without privilege/setup for Linux*

Build status
============

.. image:: https://img.shields.io/gitlab/pipeline/proot/proot.svg?label=gitlab-ci&style=flat-square
   :target: https://gitlab.com/proot/proot/pipelines

.. image:: https://img.shields.io/travis/proot-me/proot.svg?label=travis-ci&style=flat-square
   :target: https://travis-ci.org/proot-me/proot

.. image:: https://img.shields.io/badge/scan--build-latest-yellow.svg?style=flat-square
   :target: https://proot.gitlab.io/proot/reports/scan-build

.. image:: https://img.shields.io/badge/lcov-latest-6688D4.svg?style=flat-square
   :target: https://proot.gitlab.io/proot/reports/lcov

Compiling
=========

The following commands can be used to compile PRoot and CARE::

    make -C src loader.elf loader-m32.elf build.h # first build the config and loader
    make -C src proot care # then compile PRoot and CARE
    make -C test # run test suite

|asciicast|

.. |asciicast| image:: https://asciinema.org/a/315367.svg
   :target: https://asciinema.org/a/315367

Dependencies
============

- `libarchive <https://libarchive.org>`_
- `libtalloc <https://talloc.samba.org>`_
- `uthash <https://troydhanson.github.io/uthash>`_

Manuals
=======

- `PRoot <https://raw.githubusercontent.com/proot-me/proot/master/doc/proot/manual.txt>`_

- `CARE <https://raw.githubusercontent.com/proot-me/proot/master/doc/care/manual.txt>`_

Support
=======

- `Mailing List <mailto:proot_me@googlegroups.com>`_
- `Forum <https://groups.google.com/forum/?fromgroups#!forum/proot_me>`_
- `Chat <https://gitter.im/proot-me/devs>`_

License
=======

SPDX-License-Identifier: `GPL-2.0-or-later <COPYING>`_
