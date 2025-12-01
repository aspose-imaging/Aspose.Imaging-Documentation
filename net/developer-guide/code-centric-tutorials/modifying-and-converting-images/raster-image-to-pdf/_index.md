---
title: Convert Raster Image to PDF with Aspose.Imaging for .NET
linktitle: Raster Image to PDF
type: docs
weight: 30
url: /net/raster-image-to-pdf/
description: Demonstrates how to convert a raster image (e.g., GIF) into a PDF document using Aspose.Imaging for .NET.
keywords: pdf conversion c# raster-image
---

# Convert a Raster Image to PDF

## Introduction
This example shows how to load a raster image such as a GIF file and save it directly as a PDF document. It is useful when you need to embed bitmap graphics into PDF reports or archive them in a portable format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample raster image file (e.g., `sample.gif`) placed in the data directory used by the example

## Step-by-step Guide
1. Obtain the path to the folder containing the example input files.  
2. Load the raster image using `Image.Load`.  
3. Create a `PdfOptions` instance (default settings are sufficient for basic conversion).  
4. Call `image.Save` with the desired PDF file name and the `PdfOptions` object.  
5. Verify the generated PDF file in the output directory.

## Code Example
Below is the complete code snippet for this operation:

{{< gist "aspose-imaging-gists" "ddfac240600bbcd5758929cce2a3f1a4" "RasterImageToPDF.cs" >}}

## See Also
- [Convert Vector Image to PDF](/net/vector-image-to-pdf/)  
- [Apply Compression to PDF](/net/pdf-compression/)  
- [Batch Convert Images to Different Formats](/net/batch-image-conversion/)
