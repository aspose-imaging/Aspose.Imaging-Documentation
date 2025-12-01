---
title: Specify Transparency Using Raster Image (PNG)
linktitle: Specify Transparency (Raster Image)
type: docs
weight: 30
url: /net/specify-transparency-using-raster-image/
description: Demonstrates how to set background and transparent colors on a PNG image using RasterImage.
keywords: png, transparency, c#
---

# Specify Transparency Using Raster Image (PNG)

## Introduction
This example shows how to modify a PNG image by specifying its background color, transparent color, and related properties through the `RasterImage` class. Use it when you need to control PNG transparency and background handling programmatically.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A source PNG file (e.g., `aspose_logo.png`) placed in the data directory used by the example

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path that contains the input PNG file.  
2. **Load the PNG as a `RasterImage`** – Use `Image.Load` and cast the result to `RasterImage`.  
3. **Read image dimensions** – Store `Width` and `Height` if further processing is required.  
4. **Set background and transparency properties**:  
   - `BackgroundColor` – the color that fills the background (e.g., white).  
   - `TransparentColor` – the color that should become transparent (e.g., black).  
   - `HasTransparentColor` – enable transparent color handling.  
   - `HasBackgroundColor` – enable background color handling.  
5. **Save the modified image** – Export the image using `PngOptions` to a new file name.

## Code Example
The complete example is shown below:

{{< gist "aspose-imaging-gists" "45dc8b730481161bd175532a947d3bc1" "SpecifyTransparencyUsingRasterImage.cs" >}}

## See Also
- Working with PNG images in Aspose.Imaging
- Setting transparency for other image formats
- Using `RasterImage` for advanced pixel manipulation
