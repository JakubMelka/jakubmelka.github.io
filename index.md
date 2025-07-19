---
title: About
feature_text: |
  # <font face="Sans Serif">PDF4QT</font>
  <font face="Sans Serif">Unleash the power of PDF4QT: Your go-to open source PDF editor powered by the Qt framework. With a robust C++ library, intuitive PDF viewing/editing applications, and a handy command-line tool, PDF4QT streamlines your PDF interactions. Try it today.</font>
feature_image: "assets/main.png"  
excerpt: "PDF4QT is an open source PDF editor for Windows/Linux. This modern solution offers an unparalleled experience for viewing, editing, and rendering PDF documents."
---

Experience the power of PDF4QT: An open-source PDF editor designed for both Windows and Linux. This **modern solution** offers an unparalleled experience for viewing, editing, and rendering PDF documents for all users, as well as developers. Developers have access to a robust **C++ library** and a practical **command line tool** for seamless script integration. Regular users can enjoy our **four applications** packed with a wealth of features. The PDF4QT project is proudly hosted on [Github](https://github.com/JakubMelka/PDF4QT) and operates under the **LGPLv3** license. Discover the future of PDF interaction with PDF4QT today.

{% include button.html text="Github" icon="github" link="https://github.com/JakubMelka/PDF4QT" color="#0366d6" %} {% include button.html text="Tweet it" icon="twitter" link="https://twitter.com/intent/tweet/?url=https://JakubMelka.github.io&text=PDF4QT&via=JakubMelka" color="#0d94e7" %} {% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %} {% include button.html text="Donate" link="https://github.com/sponsors/JakubMelka" color="#8b0000" %}

## Goals

As the principal developer behind PDF4QT, I have set the following goals for the project:

- To create a robust foss pdf editor alternative to **commercial PDF editors**, opening up advanced PDF editing capabilities to all.
- To offer licensing terms that are more flexible than GPL or AGPL, making PDF4QT a suitable choice for both open-source enthusiasts and commercial users.
- To harness **modern C++** features and the power of **multicore CPUs**, delivering a highly efficient PDF editing experience.
- To ensure PDF4QT is inclusive and accessible, supporting applications on both Windows and Linux platforms.
- I'm actively working towards the full integration of the standard **PDF 2.0** to stay on top of the latest developments in PDF technology. While this is a work in progress, my commitment to this goal is unwavering.
- Recognizing the increasing prevalence of high-resolution monitors, I'm dedicated to ensuring PDF4QT supports 4K/8K monitors (high DPI devices) for a visually stunning user experience.

Join me on this journey and experience the power of PDF4QT today!

## Applications

Discover the power and versatility of PDF4QT's suite of applications. These tools are designed to transform the way you interact with PDF documents, offering a comprehensive set of features for viewing, editing, manipulating, and comparing PDFs. Preview our applications in the screenshots section and unlock a new level of efficiency in your workflow. Here's what we offer:

- **PDF4QT Viewer Profi**: Go beyond basic browsing. This tool packs a punch with a host of advanced features, including encryption, document reading, digital signature verification, annotation editing, and even support for searching text using regular expressions. Turn pages into images, and enhance your PDF interactions with multiple available plugins.
- **PDF4QT Viewer Lite**: Simplify your viewing experience. This lightweight viewer offers essential viewing functions in a clean, user-friendly interface.
- **PDF4QT DocPage Organizer**: Take control of your documents. Manage whole documents or individual pages with ease. Merge documents into a single file, or split them into multiple ones. You can also move, clone, or add pages with a few clicks, all within an intuitive user interface.
- **PDF4QT DocDiff**: Spot differences effortlessly. This tool allows users to open two documents and receive a detailed list of differences. View these differences in a page-to-page window where they are clearly marked. Save these differences into an XML file for future reference.

Experience the future of PDF interactions today with the PDF4QT suite of applications. Try them out now!

## Features of PDF open source reader and editor

Unleash the full potential of your PDF interactions with PDF4QT's impressive lineup of features. Designed to cater to a wide spectrum of needs, these features will revolutionize the way you handle PDFs. Here's what you can expect:

- **Multithreading Support**: Harness the power of multicore CPUs for faster, more efficient PDF processing.
- **Hardware Accelerated Rendering**: Enjoy seamless, high-quality rendering with hardware acceleration.
- **Encryption**: Ensure your documents' security with robust encryption capabilities.
- **Color Management**: Maintain the integrity and accuracy of your PDF's color profiles.
- **Optional Content Handling**: Have full control over what content to display or hide.
- **Text Layout Analysis**: This feature allows for an in-depth analysis of your existing text, enabling the conversion of PDFs into text, thereby facilitating a more efficient editing and formatting process.
- **Signature Validation**: Verify digital signatures with ease and confidence.
- **Annotations and Form Filling**: Make your PDFs interactive with annotation and form filling features.
- **Text to Speech Capability**: Access your PDFs in audio form with text to speech conversion.
- **Advanced Annotation Tools**: Enhance your PDFs by adding annotations, images, text and more.
- **File Attachments Management**: Easily view and manage the list of attached documents in your PDFs and save them to your desired location.
- **Optimization**: Reduce file size without compromising quality with document compression.
- **Command Line Tool**: Easily access and control PDF4QT via command line.
- **Audio Book Conversion**: Convert your PDFs into audio books for convenient access.
- **Internal Structure Inspector**: Understand your PDFs better with a detailed view of their internal structure.
- **Compare Documents**: Easily identify differences between similar documents.
- **Redaction**: Safeguard sensitive information by removing it from your PDFs.
- **Document Signing**: Sign your documents digitally for authenticity and validation.

- ...and much more! Delve into the world of PDF4QT and experience a new standard of handling PDFs. Test out these features today!

## Build

You should use Qt 6.4 or newer, and use the latest compiler supporting C++20. Tested compilers include MSVC, mingw, and gcc.

### Windows / Linux

To build this project, you will need:

- Qt 6.4 or newer with CMAKE 3.16 or newer
- [VCPKG](https://vcpkg.io/en/index.html) package manager
- Compiler supporting C++20 (MSVC, mingw or gcc)

Then, you can compile this project, dependencies are automatically downloaded via VCPKG. On Windows, you can also optionally create Wix project for .msi installer.

## Installation

An MSI installer is readily provided for MS Windows users, along with a ZIP archive containing all the necessary files for those who prefer to run the program without installation.
Exciting news for Linux users – AppImage and Flatpak packages are now available, offering flexible and convenient installation options across a wide range of distributions.
See the build information above if you wish to build the package yourself. Dive into the world of PDF4QT today, and transform your PDF interactions like never before.

{% include button.html text="Install PDF4QT" link="https://github.com/JakubMelka/PDF4QT/releases" color="#6cbd45" %}