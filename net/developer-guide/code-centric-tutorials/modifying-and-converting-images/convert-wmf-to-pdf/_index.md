---
title: Convert WMF to PDF using Aspose.Imaging for .NET
linktitle: Convert WMF to PDF
type: docs
weight: 30
url: /net/convert-wmf-to-pdf/
description: Shows how to load a WMF image and save it as a PDF document with rasterization options.
keywords: wmf pdf conversion c#
---

# Convert WMF to PDF

## Introduction
This example demonstrates how to load a Windows Metafile (WMF) image and save it as a PDF document using Aspose.Imaging for .NET. It is useful when you need to preserve vector graphics while generating PDF reports or documents.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A WMF file named **input.wmf** placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder that contains the input WMF file.  
2. Load the WMF image with `Image.Load`.  
3. Create a `WmfRasterizationOptions` instance and configure background color, page width, and page height.  
4. Instantiate `PdfOptions` and assign the rasterization options to its `VectorRasterizationOptions` property.  
5. Call `image.Save` with the desired PDF file name and the `PdfOptions` instance to generate the PDF.  

## Code Example
The following snippet shows the complete conversion process:

{{< gist "aspose-imaging-gists" "8e18a167a440369ba4ba36442c9b8be4" "ConvertWMFToPDF.cs" >}}

## See Also
- **Convert EMF to PDF** – another example for converting Enhanced Metafile images.  
- **Rasterize vector images** – learn how to control rasterization settings for various vector formats.  
- **Export images to PDF** – explore additional options for saving different image types as PDFs.
