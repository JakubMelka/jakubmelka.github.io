---
layout: post
title:  "Plugin Introduction"
date:   2022-07-17 17:13:12 +0100
categories: Lectures
---

PDF4QT Viewer Profi uses plugin system to provide additional features to users. There are currently seven additional plugins, which can user turn on/off in the Options dialog. They are turned off by default.

<!-- more -->

<a class="bscreenshot-link" href="/assets/posts/04-options.png" data-lightbox="annot" data-title="Options dialog with a list of plugins."><img class="bscreenshot-image" src="/assets/posts/04-options-thumb.png" alt="Options dialog with a list of plugins." /></a>

## AudioBook plugin [Windows only]

Converts PDF into an audiobook, using MS Sapi (Microsoft's library for voice synthethization). For this reason, it is available on Windows only. Audio book conversion is two phase. In
the first phase, plugin creates text stream automatically by extracting text from the PDF, and then this stream can be edited by the user (such as removing / adding text block, or modify
text extracted from the PDF). When user finish text stream editation, in the next phase, plugin AudioBook will create audio stream using voice settings in the option.

#### Features:
- automatic text extraction from text stream
- various tools how to edit text stream
- audio stream synthetization using selected voice

## Dimensions
Provides various tools to measure distance/area in PDF document. User can select metric and imperial units. Tools can be started via the toolbar.
Dimensions can be erased, they are not part of PDF document.

#### Features:
- horizontal/vertical/line dimensions
- measure angles
- 2D dimensions measuring area/perimeter

## ObjectInspector

Inspects internal structure of PDF document. Can display content of pages, fonts, images, document catalog and other object in a well organized dialog. 
Object inspector dialog uses tree navigator on the left side, and widget displaying content on the right. This plugin has availability to display object
statistics and memory consumption of these objects.

#### Features:
- display object tree in navigator using various filters
- display content of internal PDF objects, including content streams and images
- show object statistics and memory consumption

## OutputPreview

Plugin which implements PDF transparency rendering, using spot colors. It can simulate separations, paper color, or filter content via content filters -
for example, displaying of images/vector graphics can be turned off. In the output preview window, user can select which color channels are to be shown.
This plugin can also measure ink usage on the pages.

#### Features:
- render using PDF transparency model
- spot color rendering
- separation simulation
- paper color simulation
- select color channels to be shown (including shape/opacity channel)
- ink coverage warnings
- soft proofing

## Redact
Removes sensitive content from PDF document using various tools. User can select rectangle area via tool, or select text to be redacted, or redact whole pages.
This plugin cooperates with text search - results of text search can also be redacted. Plugin can redact all content except shading and tiling patterns.
Image redaction is supported - redacted content is internally deleted from the image. After the user select content to be redacted, redacted document can
be created, where sensitive content is permanently removed, and redacted area are marked as black.

#### Features:
- redact text, images and vector graphics
- various tools for content redaction
- cooperation with text search results
- create redacted document

## Signature
Sign document electronically or digitally using a certificate. User can create graphics of the signature via various tools, then sign document electronically (where there
is no reliable verification via certificate) or digitally using a certificate provided by the user. User can manage certificates via certificate manager, which can import
pfx files containing certificates.

#### Features:
- create signature graphics via various tools
- sign electronically
- sign digitally using a certificate (hiden or visible signature)
- certificate manager
- import external certificates in pfx format

## SoftProofing
Provides simple soft-proofing and gamut checking using selected icc profile.

#### Features:
- icc profile selection
- soft proofing
- gamut checking

<script src="/lightbox2/js/lightbox-plus-jquery.js"></script>
