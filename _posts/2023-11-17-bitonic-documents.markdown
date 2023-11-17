---

layout: post  
title:  "Upcoming feature: Create Bitonal Document from Scanned Pages"  
date:   2023-11-17 17:12:07 +0100  
categories: Feature
---

In the digital era, handling large scanned documents, especially from old books, poses challenges. This article introduces a new feature in my software that addresses this issue. It allows the conversion of color images in these PDFs into bitonal or black-and-white format, significantly reducing file size. The feature also offers customization options during the conversion process, giving users control over the output. Learn how this innovative feature can transform the way we manage scanned documents.

<!-- more -->

## The Overlooked Issue of Large Scanned PDF Files

Many of the older books that we find in libraries and archives have been scanned using color scanners. The PDF documents created from these scanned pages tend to be very large because they contain large, high-resolution images. These color-scanned PDFs not only take up a significant amount of disk space but also make sharing or transferring these documents a time-consuming process. The quality of these PDFs is often much higher than required for most purposes, and this excessive quality contributes to the file's large size.

## The Bitonal Solution: Black and White Pixel Conversion

The issue of large file sizes for scanned PDFs can be mitigated by converting the color images within these documents to bitonal ones. A bitonal image is a simple black and white image created using one bit per pixel. Each pixel is either black or white and no other color, therefore, drastically reducing the amount of digital data required to represent the image. By converting color images to bitonal images, the size of the resulting PDF can be reduced to about 10% of the original size. This results in smaller, more manageable files that can be easily shared and stored.

## How it looks?

<a class="bscreenshot-link" href="/assets/posts/05-bitonal.png" data-lightbox="annot" data-title="Original and bitonal image."><img class="bscreenshot-image" src="/assets/posts/05-bitonal-thumb.png" alt="Original and bitonal image." /></a>

## Upcoming Software Feature: Automated Bitonal Conversion

I am excited to announce a new feature in my software that makes this conversion process automated and user-friendly. The feature, still in the upstream, will be able to convert scanned PDFs into bitonal documents automatically, reducing the file sizes significantly. The feature is designed to be customizable so that users can specify their preferences during the conversion process.

## Customizable User Options: Selective Conversion and Threshold Determination

Users will be allowed to select which pictures should be converted and which should remain as they are. They will also be able to choose the method of conversion. For instance, they could opt for an automatic method that applies Otsu's algorithm to determine the threshold, or they could manually specify the threshold. The threshold determines the brightness value that separates black pixels from white pixels. This new feature will certainly revolutionize the way we handle and manage scanned documents, making them more accessible and convenient to use.

<script src="/lightbox2/js/lightbox-plus-jquery.js"></script>