---
title: Convert WMF to SVG with Aspose.Imaging for .NET
linktitle: Convert WMF to SVG
type: docs
weight: 30
url: /net/convert-wmf-to-svg/
description: Demonstrates how to convert a WMF image to SVG using Aspose.Imaging for .NET.
keywords: wmf svg conversion c#
---

# Convert WMF to SVG

## Introduction
This example shows how to load a WMF (Windows Metafile) image and save it as an SVG (Scalable Vector Graphics) file using Aspose.Imaging for .NET. Use it when you need to transform vector-based WMF graphics into the widely supported SVG format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A WMF sample file (e.g., `thistlegirl_wmfsample.wmf`) placed in the example data folder

## Step-by-step Guide
1. **Set up the data directory** – Obtain the path to the folder containing the input WMF file.  
2. **Load the WMF image** – Use `Image.Load` to read the WMF file into an `Image` object.  
3. **Configure rasterization options** – Create a `WmfRasterizationOptions` instance, set background color, page width, and page height based on the loaded image.  
4. **Save as SVG** – Call `image.Save` with the destination SVG file name and an `SvgOptions` object that references the rasterization options.

## Code Example
The following code demonstrates the conversion:

{{< gist "aspose-imaging-gists" "d153e2747a579cbbe1e8c49704bc7b4a" "ConvertWMFToSVG.cs" >}}

## See Also
- **Convert SVG to PNG** – Learn how to rasterize an SVG file to a PNG image.  
- **Working with Vector Images** – Overview of vector image support in Aspose.Imaging.  
- **Advanced Rasterization Options** – Explore additional settings for fine‑tuning vector rasterization.
