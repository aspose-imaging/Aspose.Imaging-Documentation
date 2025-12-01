---
title: Convert WebP Image to PDF with Aspose.Imaging for .NET
linktitle: WebP to PDF
type: docs
weight: 30
url: /net/webp-to-pdf/
description: Demonstrates how to convert a WebP image to a PDF document using Aspose.Imaging for .NET.
keywords: webp pdf conversion c#
---

# Convert WebP Image to PDF

## Introduction
This example shows how to load a WebP image and save it as a PDF document using Aspose.Imaging for .NET. It is useful when you need to embed WebP graphics into PDF reports or archives.

## Prerequisites
- .NET 9.0 (or later) development environment
- Aspose.Imaging for .NET library
- A sample WebP file (e.g., `Animation.webp`) placed in the data directory

## Step-by-step Guide
1. Obtain the path to the folder that contains the source WebP image.  
2. Load the WebP image using `Aspose.Imaging.Image.Load`.  
3. Create a `PdfOptions` instance and optionally configure PDF document information.  
4. Call the `Save` method on the loaded WebP image, specifying the output PDF file name and the `PdfOptions`.  
5. (Optional) Delete the generated PDF file after verifying the conversion.

## Code Example
The following code demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "f48bfadee9bc5a47dcf511cde1178f2b" "WebPToPdfExample.cs" >}}

## See Also
- **Convert PNG Image to PDF** – Learn how to convert PNG files to PDFs.  
- **Modify WebP Image** – Explore image manipulation techniques for WebP files.  
- **Working with PDF Options** – Configure PDF document settings such as metadata and compression.
