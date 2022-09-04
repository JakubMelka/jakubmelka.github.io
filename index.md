---
title: About PDF4QT
feature_text: |
  # <font face="Sans Serif">PDF4QT</font>
  <font face="Sans Serif">PDF4QT is open source, Qt-based PDF processing software. It contains a C++ library, applications for viewing/editing PDF documents and a command line tool.</font>
feature_image: "assets/main.png"  
excerpt: "PDF4QT is an all-in-one solution for processing PDF files in Windows/Linux. "
---

PDF4QT is an all-in-one open source software for processing PDF files in Windows/Linux. It is a **modern solution** for viewing/editing/rendering PDF documents, for users and developers alike. For developers, there is a **C++ library** and a **command line tool** for use in scripts. For users, there are **four applications** offering many features. The project is hosted on [Github](https://github.com/JakubMelka/PDF4QT) and uses license **LGPLv3**.

{% include button.html text="Github" icon="github" link="https://github.com/JakubMelka/PDF4QT" color="#0366d6" %} {% include button.html text="Tweet it" icon="twitter" link="https://twitter.com/intent/tweet/?url=https://JakubMelka.github.io&text=PDF4QT&via=JakubMelka" color="#0d94e7" %} {% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}

## Goals

The project has the following goals:

- To provide an open source alternative to **commercial pdf editors**
- To offer better licensing terms than GPL or AGPL, so it is more usable in both open source and commercial applications
- To utilize modern **C++** features and **multicore CPUs**
- To support application in Windows/Linux
- To fully integrate standard **PDF 2.0**
- To support 4K/8K monitors (high DPI devices)

## Applications

The applications are primarily used by target users to view, edit, manipulate or compare PDF documents. Users can preview these applications in the screenshots section of this webpage. There are four applications:

- **PDF4QT Viewer Profi**: Basic browsing and lots of other functionalities, such as encryption, reading a document, verification of digital signatures, editing of annotations, searching for text using regular expressions, drawing pages into an image, and much more. Several plug-ins are available.
- **PDF4QT Viewer Lite**: Simple document viewer with basic functionalities.
- **PDF4QT DocPage Organizer**: Used for the manipulation of whole documents and individual pages. Documents can be merged into one, or split into multiple ones. Pages can be (re)moved, cloned, or added. All this in an easy and intuitive user interface.
- **PDF4QT DocDiff**: Used to compare similar documents. The user opens two documents and receives a list of differences in a well-arranged list. The differences can also be viewed in a page-to-page window in which they are marked. Differences can be saved into an XML file.

## Features

The software features:

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
- redaction (removal of sensitive content)
- document signing
- .... and much more!

## Build

You should use Qt 5.15.2 or newer, and use the latest compiler supporting C++20. Tested compilers include MSVC, mingw, gcc and clang.

### Windows

In Windows, there are two options to build this software

- Use *.pro project file together with downloaded dependencies
- Use *.qbs project file which uses [Conan](https://conan.io/) to download dependencies

### Linux

In Linux, only Qbs build is supported. Download all prerequisites (Qt, Conan and compiler) and use .qbs file to compile the project.

## Installation

MSI installer is provided for MS Windows. A zip archive containing all the files is also available to be able to run the program without installation. For Linux, no installer or package is provided. However, this can be built by yourself (see build information above).

{% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}