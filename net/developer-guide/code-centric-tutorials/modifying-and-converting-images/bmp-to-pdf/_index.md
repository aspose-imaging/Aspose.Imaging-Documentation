---
title: Convert BMP Image to PDF with Aspose.Imaging for .NET
linktitle: BMP to PDF
type: docs
weight: 30
url: /net/bmp-to-pdf/
description: Demonstrates how to convert a BMP image to a PDF document using Aspose.Imaging for .NET.
keywords: bmp pdf conversion c#
---

# Convert BMP Image to PDF

## Introduction
This example shows how to load a BMP image and save it directly as a PDF document using the Aspose.Imaging library for .NET. It is useful when you need to package raster graphics into a portable, searchable PDF format without intermediate processing.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A sample BMP file (e.g., `sample.bmp`) placed in the data directory used by the examples

## Step-by-step Guide
1. **Initialize the data directory** – Resolve the folder that contains the source BMP file.
2. **Load the BMP image** – Use `Image.Load` to read the BMP file into a `BmpImage` object.
3. **Create PDF export options** – Instantiate `PdfOptions` and optionally configure document metadata via `PdfDocumentInfo`.
4. **Save the image as PDF** – Call the `Save` method on the `BmpImage` instance, passing the target PDF file path and the `PdfOptions` object.
5. **Dispose resources** – The `using` statement ensures the image is properly released after conversion.

## Code Example
The following snippet demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "c918fd1c0f61b6b93adfde05f3e3df04" "BMPToPDF.cs" >}}

## See Also
- **Convert PNG to PDF** – Learn how to convert PNG images to PDF using Aspose.Imaging.
- **Image format conversion overview** – General guidance on converting between various image formats.
- **Modifying images with Aspose.Imaging** – Techniques for editing images before conversion.
