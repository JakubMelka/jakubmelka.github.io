---
layout: post
title:  "Encrypt PDF document with strong encryption algorithm or decrypt it"
date:   2022-01-16 15:27:33 +0100
categories: Lectures
---

When you want to protect sensitive PDF document from unauthorized access, you may want to encrypt PDF document using strong encryption algorithm. PDF 2.0 standard offers two ways how to encrypt PDF Document, the first one is password protection, the latter is certificate protection. PDF4QT supports the first one, password protection using strong **AES-256** encryption, or, for backward compatibility, RC4 and AES-128 encryption.

<!-- more -->

PDF document can be protected by two passwords - user password used to open PDF document, and owner password to gain document owner access. While user password is optional, owner password is required. PDF viewers should respect permissions defined in PDF document, but nothing in PDF document enforces it - even with user password, applications can ignore the PDF specification, so access document contents is possible.

### How to encrypt/decrypt PDF document via PDF4QT Viewer Profi?

PDF4QT respects the owner's rights, so to change document encryption, it is required that you are authorized as owner (or document is not encrypted at all, so you have owner's access implicitly). From 'Edit' menu, select 'Encryption...' and encryption dialog appears, if you are authorized. Sometimes, program will ask for owner password to ensure you are authorized as owner. PDF4QT implements three encryption algorithms, but nowadays, you should always use **AES-256** algorithm, which is strongest encryption algorithm available in the PDF specification.

<a class="bscreenshot-link" href="/assets/posts/02-enc-menu.png" data-lightbox="enc02" data-title="Adjust encryption settings via menu 'Edit'."><img class="bscreenshot-image" src="/assets/posts/02-enc-menu-thumb.png" alt="Adjust encryption settings via menu 'Edit'." /></a>
<a class="bscreenshot-link" href="/assets/posts/02-enc-dlg.png" data-lightbox="enc02" data-title="Encryption settings dialog allows to change encryption settings of PDF document."><img class="bscreenshot-image" src="/assets/posts/02-enc-dlg-thumb.png" alt="Encryption settings dialog allows to change encryption settings of PDF document." /></a>

#### Encryption method
Four encryption methods are available to user:
- None (to disable encryption)
- **AES-256 (recommended)**
- AES-128 (backward compatibility)
- RC-128 (backward comaptibility)

When encryption algorithm is selected, user can enter owner's password, and (optionally) password used when document is opened. Simple password strength heuristic algorithm is shown to user as color bars indicating how secure the password is. Encryption scope (encrypt with our without metadata, encrypt only file attachments) can also be modified. Permissions can also be changed.

To decrypt PDF document, just choose 'None' option and confirm your choice by clicking OK button.

### How to encrypt/decrypt PDF document via command line?

For scripting, it is very useful to be able to encrypt/decrypt PDF document via command-line tool. Syntax is very easy. To encrypt document, you can use following command:

```
pdftool encrypt --enc-user-password=mypswd --enc-owner-password=myownerpswd --enc-permissions=8 --enc-algorithm=aes-256 document.pdf
```

To decrypt it, just use following command:

```
pdftool decrypt --pswd=myownerpswd document.pdf
```

### Remarks & tips

- encrypted document doesn't enforce permissions, applications can ignore them, once document is opened
- use strong password to protect your content, weak password can be breached
- use newest AES-256 algorithm
- use pdftool for automation via scripts
- save backup unencrypted copy of your encrypted document, if you forgot your password, then your content can be lost

<script src="/lightbox2/js/lightbox-plus-jquery.js"></script>
