---
layout: post
title:  "Welcome to PDF4QT!"
date:   2021-12-29 17:13:05 +0100
categories: General
---

Let me introduce a new software for processing PDF documents. Why to start a new project from scratch, if we have [poppler](poppler.freedesktop.org/) or [ghostscript](https://artifex.com/products/ghostscript/) and also popular viewers such as [Evince](https://wiki.gnome.org/Apps/Evince) or [Okular](https://okular.kde.org/cs/)? This software is good, but, it is quite old and also lacks many functionality comparing to commercial solutions.

<!-- more -->

For this reason, in year 2018, I have decided to start a new project - PDF4QT, which offers much more - it aims to be alternative to commercial solutions, such as **Adobe Acrobat Pro** and other feature rich programs. This year, 2021, initial version of this software was released for public testing.

## Properties
 - Provide open source alternative to commercial applications such as **Adobe Acrobat Pro** or **Foxit Software**
 - Offer better licensing terms than GPL or AGPL, so it is more usable in both open-source and commercial applications
 - Use modern **C++** features and utilize modern **multicore CPUs**
 - Support for Windows/Linux
 - Support of standard **PDF 2.0**
 
## Future long-term goals
These goals I would like to achieve in probably two years:
 - document signing
 - watermarks
 - 3D PDF support
 - XFA support (static forms only)
 - form editing (AcroForms only)
 - OCR
 - presentation application
 - application managing collection of PDF documents
 - full support of standard PDF 2.0
 
## What is unique?
I have also implemented some features, which are unique to this project among other open source project (but commercial applications, of course, implement them). The first one noted, is **PDF4QT DocDiff** which can compare two similar PDF documents, on content basis. It examines content of both PDF documents and displays results of this comparison in well-formed GUI. Advanced algorithms are used for comparison, text is compared as whole and not per page basis, so it can handle text moving (for example, paragraph is on a new page in the second document), and images and vector graphics are also compared.
 
The second one, is **redaction** (remove of sensitive content from the PDF document), in a form of plugin. User can use various tools to mark areas of the page to be redacted. Text can be selected by mouse, also rectangle area (useful for image redacting) and whole pages can be redacted. In addition, user can use search results to redact multiple text occurences (also regular expressions can be used). Then user can create redacted document where sensitive content is removed (works also for images).
 
The third one, is **audio book creation**, also in a form of plugin. This plugin has following workflow: user creates text stream with text blocks, which will be then transformed into an audio stream. Text stream is automatically created by collecting text blocks from the PDF document (it is better to have tagged PDF). User can add or remove text blocks from the audio stream, or modify them. When text stream is prepared, audio stream can be created from it.
