---
title: Draw a Raster Image onto a WMF Vector Image with Aspose.Imaging for .NET
linktitle: Draw Raster on WMF
type: docs
weight: 30
url: /net/draw-raster-image-on-wmf/
description: Demonstrates how to draw a raster image onto a WMF vector canvas using Aspose.Imaging for .NET.
keywords: draw raster wmf c#
---

# Draw a Raster Image onto a WMF Vector Image

## Introduction
This example shows how to embed a raster image into a WMF (Windows Metafile) vector image using Aspose.Imaging for .NET. It is useful when you need to combine bitmap graphics with vector-based drawings in a single WMF file.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample raster image (`asposenet_220_src01.png`) and WMF canvas file (`asposenet_222_wmf_200.wmf`) located in the data folder

## Step-by-step Guide
1. Obtain the data directory that contains the source raster and WMF files.  
2. Load the raster image using `Image.Load` and cast it to `RasterImage`.  
3. Load the WMF file that will serve as the drawing surface and cast it to `WmfImage`.  
4. Create a `WmfRecorderGraphics2D` instance from the WMF image.  
5. Call `graphics.DrawImage` to draw the raster image onto the WMF canvas, specifying source and destination rectangles.  
6. End the recording with `graphics.EndRecording()` to obtain the resulting `WmfImage`.  
7. Save the resulting WMF file to the desired location.

## Code Example
The following code snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "9ce1b33e54420f16f1534ec4a831b928" "DrawRasterImageOnWMF.cs" >}}

## See Also
- **Convert Raster Images to Vector Formats** – Learn how to convert bitmap images to vector formats using Aspose.Imaging.  
- **Create and Manipulate WMF Files** – Explore creating WMF files from scratch and adding vector graphics.  
- **Apply Transformations to Images** – Apply scaling, rotation, and other transformations to images before drawing.
