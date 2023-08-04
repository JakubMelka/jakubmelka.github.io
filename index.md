---
title: About PDF4QT
feature_text: |
  # <font face="Sans Serif">PDF4QT</font>
  <font face="Sans Serif">Unleash the power of PDF4QT: Your go-to open source PDF editor powered by the Qt framework. With a robust C++ library, intuitive PDF viewing/editing applications, and a handy command-line tool, PDF4QT streamlines your PDF interactions. Try it today.</font>
feature_image: "assets/main.png"  
excerpt: "PDF4QT is an open source PDF editor for Windows/Linux. "
---

Experience the power of PDF4QT: An open-source PDF editor designed for both Windows and Linux. This **modern solution** offers an unparalleled experience for viewing, editing, and rendering PDF documents for all users, as well as developers. Developers have access to a robust **C++ library** and a practical **command line tool** for seamless script integration. Regular users can enjoy our **four applications** packed with a wealth of features. The PDF4QT project is proudly hosted on [Github](https://github.com/JakubMelka/PDF4QT) and operates under the **LGPLv3** license. Discover the future of PDF interaction with PDF4QT today.

{% include button.html text="Github" icon="github" link="https://github.com/JakubMelka/PDF4QT" color="#0366d6" %} {% include button.html text="Tweet it" icon="twitter" link="https://twitter.com/intent/tweet/?url=https://JakubMelka.github.io&text=PDF4QT&via=JakubMelka" color="#0d94e7" %} {% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}

## Goals

As the principal developer behind PDF4QT, I have set the following goals for the project:

- To create a robust open-source alternative to **commercial PDF editors**, opening up advanced PDF editing capabilities to all.
- To offer licensing terms that are more flexible than GPL or AGPL, making PDF4QT a suitable choice for both open-source enthusiasts and commercial users.
- To harness **modern C++** features and the power of **multicore CPUs**, delivering a highly efficient PDF editing experience.
- To ensure PDF4QT is inclusive and accessible, supporting applications on both Windows and Linux platforms.
- I'm actively working towards the full integration of the standard **PDF 2.0** to stay on top of the latest developments in PDF technology. While this is a work in progress, my commitment to this goal is unwavering.
- Recognizing the increasing prevalence of high-resolution monitors, I'm dedicated to ensuring PDF4QT supports 4K/8K monitors (high DPI devices) for a visually stunning user experience.

Join me on this journey and experience the power of PDF4QT today!

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

You should use Qt 6.4 or newer, and use the latest compiler supporting C++20. Tested compilers include MSVC, mingw, and gcc.

### Windows / Linux

To build this project, you will need:

- Qt 6.4 or newer with CMAKE 3.16 or newer
- [VCPKG](https://vcpkg.io/en/index.html) package manager
- Compiler supporting C++20 (MSVC, mingw or gcc)

Then, you can compile this project, dependencies are automatically downloaded via VCPKG. On Windows, you can also optionally create Wix project for .msi installer.

## Installation

MSI installer is provided for MS Windows. A zip archive containing all the files is also available to be able to run the program without installation. For Linux, no installer or package is provided. However, this can be built by yourself (see build information above).

{% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}