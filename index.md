---
title: About PDF4QT
feature_text: |
  # <font face="Sans Serif">PDF4QT</font>
  <font face="Sans Serif">PDF4QT is open source Qt-based PDF processing software. It contains C++ library and applications for viewing/editing PDF documents and a command line tool.</font>
feature_image: "assets/main.png"
excerpt: "PDF4QT is all-in-one solution for processing PDF files on Windows/Linux. "
---

PDF4QT is all-in-one open source software for processing PDF files on Windows/Linux. It's goal is to provide a **modern solution** for viewing/editing/rendering PDF documents both for users and developers. For developers, there is a **C++ library and** a **command line tool**, which can be used in scripts. For users, there are **four applications** offering many features. Project is hosted on [Github](https://github.com/JakubMelka/PDF4QT) and uses license **LGPLv3**.

{% include button.html text="Github" icon="github" link="https://github.com/JakubMelka/PDF4QT" color="#0366d6" %} {% include button.html text="Tweet it" icon="twitter" link="https://twitter.com/intent/tweet/?url=https://JakubMelka.github.io&text=PDF4QT&via=JakubMelka" color="#0d94e7" %} {% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}

## Goals

Project aims to match these goals:
 - Provide open source alternative to **commercial pdf editors** 
 - Offer better licensing terms than GPL or AGPL, so it is more usable in both open-source and commercial applications
 - Use modern **C++** features and utilize modern **multicore CPUs**
 - Support for Windows/Linux
 - Full support of standard **PDF 2.0**
 - 4K/8K monitor support (high DPI devices)
 
## Applications

Applications are primarily used by target users to view, edit, manipulate or compare PDF documents. User can preview these applications
in the screenshots section of this web-page. There are four applications, each is targetting different features:

- **PDF4QT Viewer Profi**: In addition to basic browsing, it offers a lot of other functionality, such as encryption, reading a document, verifying digital signatures, editing annotations, searching for text using regular expressions, drawing pages into an image, and many other functions. Several plugins for this application are available.
- **PDF4QT Viewer Lite**: Simple document viewer with basic functionality.
- **PDF4QT DocPage Organizer**: This program is used to manipulate document pages and whole documents. Documents can be merged into one, or splitted into multiple ones. Pages can be removed, cloned, moved or added. All these in easy and intuitive user interface.
- **PDF4QT DocDiff**: Used to compare similar documents. User opens two documents and receives a list of differences in a well-aranged list. Also, user can view these differences in page-to-page view window, where they are marked. Differences can be saved into XML file.

## Features

Software has following major features:

- multithreading support
- hardware accelerated rendering
- encryption
- color management
- optional content handling
- text layout analysis
- signature validation
- annotations
- form filling
- text to speech capability
- editation
- file attachments
- optimalization (compressing documents)
- command line tool
- audio book conversion
- internal structure inspector
- compare documents
- redaction (remove sensitive content)
- document signing
- many other!

## Build
Generally, you should use Qt 5.15.2 or newer, and use latest compiler supporting C++20. Tested compilers include MSVC, mingw, gcc and clang.

### Windows

On Windows, there are two options to build this software
 - Use *.pro project file together with dependencies downloaded
 - Use *.qbs project file which uses [Conan](https://conan.io/) to download dependencies
 
### Linux

On Linux, only Qbs build is supported. Download all prerequisites (Qt, Conan and compiler) and use .qbs file to
compile the project.

## Installation

MSI installator is provided for MS Windows, and zip archive is available with all files to be able to run program without installation. For Linux, no installator or package is provided, but you can build it on your own (see build information above).

{% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}



