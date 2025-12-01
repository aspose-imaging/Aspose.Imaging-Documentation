---
title: Convert ODG Files to PNG and PDF with Aspose.Imaging
linktitle: ODG to PNG/PDF
type: docs
weight: 30
url: /net/support-for-odg/
description: Demonstrates how to rasterize ODG files to PNG and PDF using Aspose.Imaging for .NET.
keywords: odg conversion c#
---

# Convert ODG Files to PNG and PDF with Aspose.Imaging

## Introduction
This example shows how to load OpenDocument Graphic (ODG) files and rasterize them into PNG and PDF formats. Use it when you need to convert vector‑based ODG images to raster or document formats in .NET applications.

## Prerequisites
- .NET 6.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- Sample ODG files (`example.odg`, `example1.odg`) placed in a folder you can access

## Step-by-step Guide
1. **Prepare the input folder** – Define the path that contains the ODG files you want to convert.  
2. **Create rasterization options** – Instantiate `OdgRasterizationOptions` and set the page size based on the source image.  
3. **Load each ODG file** – Use `Image.Load` to open the file.  
4. **Save as PNG** – Call `Image.Save` with `PngOptions`, passing the rasterization options.  
5. **Save as PDF** – Call `Image.Save` again, this time with `PdfOptions`, using the same rasterization settings.  
6. **Repeat for all files** – Loop through the list of ODG files to generate both PNG and PDF outputs.

## Code Example
The following snippet contains the complete implementation of the steps described above.

{{< gist "aspose-imaging-gists" "d7e5a0e314402cbc281216857459ed95" "SupportForODG.cs" >}}

## See Also
- [Rasterizing Vector Images with Aspose.Imaging](#)
- [Saving Images in Different Formats (PNG, JPEG, TIFF)](#)
- [Working with PDF Options in Aspose.Imaging](#)
