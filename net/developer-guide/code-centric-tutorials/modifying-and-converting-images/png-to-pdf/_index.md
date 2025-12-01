---
title: Convert PNG Image to PDF Using Aspose.Imaging for .NET
linktitle: PNG to PDF
type: docs
weight: 30
url: /net/png-to-pdf/
description: Demonstrates how to convert a PNG image to a PDF document with Aspose.Imaging for .NET.
keywords: png pdf c#
---

# Convert PNG Image to PDF

## Introduction
This example illustrates how to load a PNG image and save it as a PDF file using Aspose.Imaging for .NET. It is useful when you need to bundle raster images into a PDF document for easier distribution or printing.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample PNG file (e.g., `sample.png`) placed in the example's data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the sample PNG image.  
2. Load the PNG image using `Image.Load` and cast it to `PngImage`.  
3. Create an instance of `PdfOptions` and optionally configure PDF document settings.  
4. Call the `Save` method on the `PngImage` object, specifying the output PDF file name and the `PdfOptions` instance.  
5. Release resources by disposing the image object (handled automatically with a `using` block).

## Code Example
The following code demonstrates the conversion:

{{< gist "aspose-imaging-gists" "66ca29dbe794df82d0293b5cb38d9230" "PNGtoPDF.cs" >}}

## See Also
- [Convert JPEG Image to PDF](#)  
- [Modify Image Properties with Aspose.Imaging](#)  
- [Working With PDF Options in Aspose.Imaging](#)
