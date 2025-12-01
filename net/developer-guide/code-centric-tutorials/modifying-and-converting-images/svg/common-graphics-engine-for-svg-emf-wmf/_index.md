---
title: Using CommonGraphicsEngine for SVG, EMF, and WMF in Aspose.Imaging for .NET
linktitle: CommonGraphicsEngine for SVG
type: docs
weight: 30
url: /net/common-graphics-engine-for-svg-emf-wmf/
description: Demonstrates how to draw vector graphics on an SVG image using Aspose.Imaging for .NET.
keywords: svg drawing c#
---

# Using CommonGraphicsEngine for SVG, EMF, and WMF

## Introduction
This example shows how to employ the `CommonGraphicsEngineForSvgEmfWmf` class to draw basic shapes, text, and other vector graphics directly onto an SVG image. It is useful when you need to generate or modify SVG content programmatically before converting it to other vector formats such as EMF or WMF.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- No external image files are required; the example creates an SVG image in memory

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder where temporary files will be stored.
2. **Create a new `SvgImage`** – Instantiate a `VectorImage` with a specified width and height.
3. **Initialize a `Graphics` object** – Attach the graphics engine to the vector image.
4. **Draw shapes and text** – Use methods such as `FillRectangle`, `DrawEllipse`, `DrawPie`, `DrawLine`, `DrawString`, etc., to render the desired graphics.
5. **Save the SVG file** – Persist the modified vector image to a file path.
6. **Clean up** – Delete the generated SVG file after processing to keep the workspace tidy.

## Code Example
The complete source code for this example is shown below:

{{< gist "aspose-imaging-gists" "f152af77a738df64a75ea45701f5ac47" "CommonGraphicsEngineForSvgEmfWmf.cs" >}}

## See Also
- Creating SVG images with Aspose.Imaging
- Converting SVG to PNG, JPEG, or other raster formats
- Using the `Graphics` class for raster image manipulation
