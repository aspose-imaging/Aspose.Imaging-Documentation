---
title: Embedding and Verifying Digital Signatures in Images
linktitle: Digital Signature Support
type: docs
weight: 30
url: /net/support-of-digital-signature/
description: Demonstrates how to embed and check a digital signature in a PNG image using Aspose.Imaging for .NET.
keywords: digital signature c#
---

# Embedding and Verifying Digital Signatures in Images

## Introduction
This example shows how to embed a digital signature into an image and subsequently verify its presence using Aspose.Imaging for .NET. Use it when you need to protect image authenticity or detect tampering.

## Prerequisites
- .NET 9.0 (or any compatible .NET version)  
- Aspose.Imaging for .NET library installed  
- A PNG image file to work with (the example uses `00020.png`)

## Step-by-step Guide
1. Locate the directory that contains the source image.  
2. Load the image as a `RasterImage` using `Image.Load`.  
3. Call `EmbedDigitalSignature(password)` to embed the signature.  
4. Verify the signature with `IsDigitalSigned(password)`.  
5. Output the verification result to the console.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "c26a5135de64f09911ec344b49f5d338" "SupportOfDigitalSignature.cs" >}}

## See Also
- **Adding Watermarks to Images** – Learn how to overlay text or image watermarks.  
- **Steganography with LSB** – Explore embedding hidden data using the least‑significant‑bit technique.  
- **Image Encryption** – Secure entire images with encryption features provided by Aspose.Imaging.
