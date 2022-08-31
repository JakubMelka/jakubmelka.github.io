---

layout: post  
title:  "Introduction to plug-ins"  
date:   2022-07-16 17:13:12 +0100  
categories: Lectures
---

PDF4QT Viewer Profi uses plug-ins to provide additional features to users. There are currently seven plug-ins, which the user can turn on/off in the Options dialog. They are turned off by default.

<!-- more -->
<a class="bscreenshot-link" href="/assets/posts/04-options.png" data-lightbox="annot" data-title="Options dialog with a list of plugins."><img class="bscreenshot-image" src="/assets/posts/04-options-thumb.png" alt="Options dialog with a list of plugins." /></a>

## AudioBook plug-in \[Windows only]

Converts PDF into an audiobook using MS Sapi (Microsoft's library for voice synthesization). For this reason, it is only available in Windows. Audio book conversion is two phase. In the first phase, the plug-in creates a text stream automatically by extracting text from the PDF, which can then be edited by the user (such as removing / adding a text block, or modifying text extracted from the PDF). In the next phase, when the user has finished editing the text stream, the AudioBook plug-in creates an audio stream using the voice settings in the option.

#### Features:

- automatic text extraction from a text stream
- various tools to edit a text stream
- audio stream synthesization using a selected voice

## Dimensions

Provides various tools to measure distance/area in PDF document. User can select metric and imperial units. Tools can be started via the toolbar. Dimensions can be erased; they are not part of the PDF document.

#### Features:

- horizontal/vertical/line dimensions
- angle measurement
- 2D dimensions measuring area/perimeter

## ObjectInspector

Inspects the internal structure of a PDF document. Can display the content of pages, fonts, images, document catalog and other objects in a well organized dialog. Object inspector dialog uses a tree navigator on the left, and a widget content display on the right. This plug-in also displays object statistics and memory consumption.

#### Features:

- displays object tree in navigator using various filters
- displays content of internal PDF objects, including content streams and images
- displays object statistics and memory consumption

## OutputPreview

Plug-in which enables PDF transparency rendering, using spot colors. It can simulate separations, paper color, or filter content via content filters - for example, the display of images/vector graphics can be turned off. In the output preview window, the user can select which color channels are to be shown. This plug-in can also measure ink usage on the pages.

#### Features:

- rendering using PDF transparency model
- spot color rendering
- separation simulation
- paper color simulation
- color channel selection (including shape/opacity channel)
- ink coverage warnings
- soft proofing

## Redact

Removes sensitive content from a PDF document using various tools. The user can select a rectangular area with a tool, or select text to be redacted, or redact whole pages. This plug-in cooperates with text search - the results of a text search can also be redacted. The plug-in can redact all content, with exception to shading and tiling patterns. Image redaction is supported - redacted content is internally deleted from the image. After the user has selected the content to be redacted, a redacted document can be created in which any sensitive content is permanently removed, with the redacted area marked as black.

#### Features:

- redaction of text, images and vector graphics
- various tools for content redaction
- cooperates with text search results
- creation of redacted document

## Signature

Sign documents electronically or digitally using a certificate. The user can create graphics of their signature using various tools, then sign documents electronically (where there is no reliable verification via a certificate) or digitally using a certificate provided by the user. The user can manage certificates via certificate manager, which can import pfx files containing certificates.

#### Features:

- create signature graphics using various tools
- sign electronically
- sign digitally using a certificate (hidden or visible signature)
- certificate manager
- import external certificates in pfx format

## SoftProofing

Provides simple soft proofing and gamut checking using a selected icc profile.

#### Features:

- icc profile selection
- soft proofing
- gamut checking

<script src="/lightbox2/js/lightbox-plus-jquery.js"></script>
