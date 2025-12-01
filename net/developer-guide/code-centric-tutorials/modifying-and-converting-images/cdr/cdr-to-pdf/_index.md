---
title: Convert CDR Image to PDF with Aspose.Imaging for .NET
linktitle: CDR to PDF
type: docs
weight: 30
url: /net/cdr-to-pdf/
description: Demonstrates how to convert a CorelDRAW (CDR) file to PDF using Aspose.Imaging for .NET.
keywords: cdr pdf conversion
---

# Convert CDR Image to PDF

## Introduction
This example shows how to load a multi‑page CorelDRAW (CDR) file and export it as a PDF document. Use it when you need to generate PDF reports or share vector drawings in a widely supported format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample CDR file (e.g., `MultiPage2.cdr`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the directory containing the input CDR file.  
2. Load the CDR file as a `VectorMultipageImage`.  
3. Create rasterization options for each page using `VectorRasterizationOptions`.  
4. Configure `PdfOptions` with the page rasterization options.  
5. Save the image to PDF using `image.Save(outputPath, pdfOptions)`.  
6. Optionally delete the generated PDF after verification.

## Code Example
The following snippet demonstrates the complete conversion flow:

{{< gist "aspose-imaging-gists" "e3758f20304dd36171a63440fa167af3" "CdrToPdfExmple.cs" >}}

## See Also
- **Convert CDR to PNG** – learn how to export CorelDRAW files to raster image formats.  
- **Working with Vector Images** – explore handling of vector graphics with Aspose.Imaging.  
- **Multi‑page PDF Generation** – combine multiple images into a single PDF document.
