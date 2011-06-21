=========================================
buildpkg -- build rpm package from PKGDEF
=========================================

buildpkg is simple wrapper for `fpm`_ to build rpm package from PKGDEF -
ArchLinux's PKGBUILD-like build script file.

It's target user is lazy sysadmin, who need to install software that is not
packaged by his distribution but don't want to learn/remember how to write
spec file.

.. _`fpm`: https://github.com/jordansissel/fpm

usage
=====

::

  $ mkdir package-name
  $ cd package-name
  $ cp /path/to/buildpkg/PKGDEF.proto PKGDEF
  $ vim PKGDEF
  $ /path/to/buildpkg/buildpkg
