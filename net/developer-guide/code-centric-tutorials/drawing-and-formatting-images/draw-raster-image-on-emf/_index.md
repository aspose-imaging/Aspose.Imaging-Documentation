---
title: Draw a Raster Image onto an EMF Vector Canvas
linktitle: Draw Raster on EMF
type: docs
weight: 30
url: /net/draw-raster-image-on-emf/
description: Demonstrates how to draw a raster image onto an EMF vector image using Aspose.Imaging for .NET.
keywords: draw image emf c#
---

# Draw a Raster Image onto an EMF Vector Canvas

## Introduction
This example shows how to load a raster image and render it onto an EMF (Enhanced Metafile) vector canvas. Use it when you need to combine raster graphics with vector formats for high‑quality scaling or printing.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample raster image (`asposenet_220_src01.png`) and EMF template (`input.emf`) placed in the example data folder

## Step-by-step Guide
1. Obtain the data directory that contains the sample images.  
2. Load the raster image (`RasterImage`) using `Image.Load`.  
3. Load the EMF image (`EmfImage`) that will serve as the drawing surface.  
4. Create an `EmfRecorderGraphics2D` object from the EMF image.  
5. Call `graphics.DrawImage` to draw the raster image onto the EMF canvas, specifying source and destination rectangles.  
6. End the recording to obtain the resulting EMF image.  
7. Save the resulting EMF file to the output path.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "fa1f1491f8a49afa2caa723470211acf" "DrawRasterImageOnEMF.cs" >}}

## See Also
- **Convert Raster to Vector Formats** – Learn how to convert raster images to various vector formats.  
- **Manipulate EMF Images** – Explore other drawing and editing operations on EMF files.  
- **Advanced Graphics with Aspose.Imaging** – Dive deeper into graphics transformations and rendering techniques.
