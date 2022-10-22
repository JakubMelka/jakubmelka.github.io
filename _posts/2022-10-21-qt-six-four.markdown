---

layout: post  
title:  "Build system changed to CMAKE, move to Qt 6.4"  
date:   2022-10-21 12:29:53 +0100  
categories: General
---

There is a major change in the build system, which now works both for Windows/Linux. Project now uses CMAKE and Qt 6.4.

<!-- more -->

## Build system

In previous versions, there were two build systems - .pro and .qbs with conan package manager. Project is now united to use CMAKE
and Qt 6.4 or newer. Dependencies are now automatically downloaded via VCPKG package manager both on linux and windows.

## Tested compiles

You can use these compilers to compile this project:

 - MSVC 2022 (version 17.1) or newer (Windows)
 - mingw 11.2.0 or newer (Windows)
 - gcc 11.2.0 or newer (Linux)
 
A lot of effort has been made to remove all compiler warnings from the code.

## Move to Qt 6.4

Project PDF4QT now uses Qt 6.4, which supports all features needed by PDF4QT.