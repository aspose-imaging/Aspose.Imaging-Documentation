---
title: Draw Raster Image on SVG using Aspose.Imaging for .NET
linktitle: Draw raster on SVG
type: docs
weight: 30
url: /net/draw-raster-image-on-svg/
description: Demonstrates how to draw a raster image onto an existing SVG canvas using Aspose.Imaging for .NET.
keywords: svg draw raster c#
---

# Draw Raster Image on SVG

## Introduction
This example shows how to load a raster image and render it onto an existing SVG canvas.  
It is useful when you need to combine bitmap graphics with vector graphics in a single image file.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0 but works on any supported version)
- Aspose.Imaging for .NET library
- Input files: a raster PNG image (`asposenet_220_src01.png`) and an SVG file (`asposenet_220_src02.svg`) located in the example data folder

## Step-by-step Guide
1. **Load the raster image** using `Image.Load` and cast it to `RasterImage`.
2. **Load the SVG canvas** with `Image.Load` and cast it to `SvgImage`.
3. Create an instance of `SvgGraphics2D` for the SVG canvas.
4. Call `graphics.DrawImage` specifying source and destination rectangles to place the raster image onto the SVG.
5. End the recording with `graphics.EndRecording()` to obtain the resulting `SvgImage`.
6. Save the resulting SVG to a new file.

## Code Example
The following code demonstrates the complete example:

{{< gist "aspose-imaging-gists" "f4a178db9aefb75b5fc502b016053beb" "DrawRasterImageOnSVG.cs" >}}

## See Also
- Working with SVG images in Aspose.Imaging
- Converting raster images to vector formats
- Manipulating image graphics with Aspose.Imaging for .NET
