---
layout: post  
title:  "Welcome to PDF4QT"
date:   2021-12-29 17:13:05 +0100  
categories: General
---

I would like to introduce new software for processing PDF documents. Why start a new project from scratch when we already have [poppler](poppler.freedesktop.org/) or [ghostscript,](https://artifex.com/products/ghostscript/) and also popular viewers such as [Evince](https://wiki.gnome.org/Apps/Evince) or [Okular](https://okular.kde.org/cs/)? All of these are good, but are quite old and lack many functionalities compared to commercial solutions.

<!-- more -->
It is for this reason that, in 2018, I decided to start a new project - PDF4QT. PDF4QT offers much more - it aims to be an alternative to commercial pdf editors. The initial version of the software was released for public testing in 2021.

## Properties

- It is an open source alternative to **commercial pdf editors**
- It offers better licensing terms than GPL or AGPL, so it is more usable in both open source and commercial applications
- It utilizes modern **C++** features and **multicore CPUs**
- It is supported in Windows/Linux
- It uses standard **PDF 2.0**

## Future long-term goals

I would like to achieve the following goals in the next two years:

- document signing
- watermarks
- 3D PDF support
- XFA support (static forms only)
- form editing (AcroForms only)
- OCR
- presentation application
- application managing the collection of PDF documents
- fully supported by standard PDF 2.0

## What is unique?

I have implemented some features that are unique to this project compared to other open source projects (commercial applications, of course, implement them). The first is **PDF4QT DocDiff**, which can compare two similar PDF documents on the basis of content. It examines the content of both PDF documents and displays the results of the comparison in a well-formed GUI. Advanced algorithms are used for the comparison. The text is compared as a whole, not on a per page basis, so it can handle text movements (e.g. a paragraph is on a new page in the second document). Images and vector graphics are also compared.

The second is **redaction** (removal of sensitive content from a PDF document), which comes in the form of a plug-in. The user can use various tools to mark areas of the page to be redacted. The text can be selected using a mouse. A rectangular area (useful for image redacting) and whole pages can also be redacted. Users can also use search results to redact multiple text occurences (also regular expressions can be used), as well as create redacted documents in which sensitive content has been removed (works also for images).

The third is **audio book creation**, which also comes in the form of a plug-in. This plug-in has the following workflow: the user creates a text stream with text blocks, which are then transformed into an audio stream. The text stream is automatically created by collecting text blocks from the PDF document (it is better to have a tagged PDF). The user can add or delete text blocks from the audio stream, or modify them. When a text stream has been prepared, audio stream can be created from it.