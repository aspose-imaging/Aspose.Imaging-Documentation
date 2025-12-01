---
title: Support for JPEG‑LS Format
linktitle: JPEG‑LS Support
type: docs
weight: 10
url: /net/support-for-jpeg-ls-format/
description: Demonstrates decoding JPEG‑LS images and saving them as PNG using Aspose.Imaging for .NET.
keywords: jpeg ls c#
---

# Support for JPEG‑LS Format

## Introduction
This example shows how to load a JPEG‑LS image, read its JPEG‑LS specific options, and convert the image to PNG format. It also demonstrates how to save a selected region of the original image. Use this guide when you need to work with lossless JPEG‑LS files in your .NET applications.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- A JPEG‑LS image file (e.g., `lena24b.jls`) and write access to an output directory

## Step-by-step Guide
1. **Set up file paths** – Determine the source JPEG‑LS file and the output PNG file locations.  
2. **Load the JPEG‑LS image** – Use `Image.Load` and cast the result to `JpegImage`.  
3. **Read JPEG‑LS options** – Access the `JpegOptions` property to inspect compression type, allowed lossy error, interleave mode, and sampling information.  
4. **Save the full image as PNG** – Call `jpegImage.Save` with a new `PngOptions` instance.  
5. **Save a region of the image** – Define a `Rectangle` for the bottom‑right quarter of the image and pass it to `jpegImage.Save` along with `PngOptions` to create a cropped PNG file.

## Code Example
The following code demonstrates the complete workflow:
{{< gist "aspose-imaging-gists" "ac22b66be78b2afa656e6eb8939785b5" "SupportForJPEG-LSFormat.cs" >}}

## See Also
- Converting JPEG images to other formats
- Working with JPEG options in Aspose.Imaging
- Reading and writing PNG images with Aspose.Imaging
