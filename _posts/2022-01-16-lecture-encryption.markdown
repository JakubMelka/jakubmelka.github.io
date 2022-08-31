---
layout: post  
title:  "Encrypting a PDF document with a strong encryption algorithm or decrypting it"  
date:   2022-01-16 15:27:33 +0100  
categories: Lectures
---

When you want to protect a sensitive PDF document from unauthorized access, you may want to encrypt it using a strong encryption algorithm. Standard PDF 2.0 offers two ways to encrypt a PDF document. The first is password protection, the second certificate protection. PDF4QT supports the first option by utilizing strong **AES-256** encryption, or for backward compatibility, RC4 and AES-128 encryption.

<!-- more -->
A PDF document can be protected by two passwords - a user password used to open the PDF document, and an owner password for the owner to gain access to the document. The user password is optional, whereas the owner password is required. Viewers of a PDF document should respect the permissions specified in the PDF document. However, nothing in the PDF document enforces this - even with a user password, applications can ignore the PDF specifications, thereby making access to document contents possible.

### How do you encrypt/decrypt a PDF document via PDF4QT Viewer Profi?

PDF4QT respects the owner's rights. In order to change a document's encryption, it is necessary to be authorized as the owner. Alternatively, the document is not encrypted, so you implicitly have owner's access. From the 'Edit' menu, select 'Encryption...'. If you are authorized, the encryption dialog appears. On occasions, the program will ask for the owner password to ensure you are authorized as the owner. Although PDF4QT implements three encryption algorithms, you should always utilize the **AES-256** algorithm, which is strongest encryption algorithm available in the PDF specification.

<a class="bscreenshot-link" href="/assets/posts/02-enc-menu.png" data-lightbox="enc02" data-title="Adjust encryption settings via menu 'Edit'."><img class="bscreenshot-image" src="/assets/posts/02-enc-menu-thumb.png" alt="Adjust encryption settings via menu 'Edit'." /></a>
<a class="bscreenshot-link" href="/assets/posts/02-enc-dlg.png" data-lightbox="enc02" data-title="Encryption settings dialog allows to change encryption settings of PDF document."><img class="bscreenshot-image" src="/assets/posts/02-enc-dlg-thumb.png" alt="Encryption settings dialog allows to change encryption settings of PDF document." /></a>

#### Encryption method

Four encryption methods are available:

- None (to disable encryption)
- **AES-256 (recommended)**
- AES-128 (backward compatibility)
- RC-128 (backward comaptibility)

When an encryption algorithm has been selected, the user can enter the owner password, and (optionally) a user password to open the document. A simple heuristic algorithm tests password strength. How secure a password is, is represented to users by color bars. The scope of encryption (encrypt with our without metadata, encrypt only file attachments) can also be modified. Permissions can also be changed.

To decrypt a PDF document, select the 'None' option and confirm your choice by clicking OK.

### How do you encrypt/decrypt a PDF document via a command line?

For scripting, it is very useful to be able to encrypt/decrypt a PDF document using the command-line tool. Syntax is very easy. To encrypt a document, use the following command:

```
pdftool encrypt --enc-user-password=mypswd --enc-owner-password=myownerpswd --enc-permissions=8 --enc-algorithm=aes-256 document.pdf
```

To decrypt a document, use the following command:

```
pdftool decrypt --pswd=myownerpswd document.pdf
```

### Remarks & tips

- an encrypted document does not enforce permissions; applications can ignore them once a document has been opened
- use a strong password to protect your content; weak passwords can be breached
- use the newest AES-256 algorithm
- use pdftool for automation via scripts
- save a backup of the unencrypted version of your encrypted document; if you forget your password, your content may be lost

<script src="/lightbox2/js/lightbox-plus-jquery.js"></script>
