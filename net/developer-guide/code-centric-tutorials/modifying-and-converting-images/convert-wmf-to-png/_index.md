---
title: Convert WMF to PNG using Aspose.Imaging for .NET
linktitle: Convert WMF to PNG
type: docs
weight: 30
url: /net/convert-wmf-to-png/
description: Demonstrates how to convert a WMF vector image to PNG using Aspose.Imaging for .NET.
keywords: wmf png c#
---

# Convert WMF to PNG

## Introduction
This example shows how to load a WMF (Windows Metafile) image and rasterize it into a PNG file using Aspose.Imaging for .NET. Use it when you need to transform vector WMF graphics into raster PNG format for web or UI consumption.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A WMF sample file (e.g., `thistlegirl_wmfsample.wmf`) placed in the data directory used by the examples

## Step-by-step Guide
1. Obtain the path to the directory that contains the source WMF file.  
2. Load the WMF image with `Image.Load`.  
3. Configure `WmfRasterizationOptions` to set background color, page width, and page height.  
4. Save the loaded image as PNG using `image.Save` with a `PngOptions` instance that references the rasterization options.  
5. Verify the output PNG file is created in the target location.

## Code Example
The following snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "654ea61d1c2a0d20585b54cce3d7e2a2" "ConvertWMFToPNG.cs" >}}

## See Also
- **Convert SVG to PNG** – Learn how to rasterize SVG vector graphics to PNG.  
- **Convert EMF to PNG** – Example for converting EMF files to raster PNG images.  
- **Working with Image Options** – Overview of different image options available in Aspose.Imaging.
