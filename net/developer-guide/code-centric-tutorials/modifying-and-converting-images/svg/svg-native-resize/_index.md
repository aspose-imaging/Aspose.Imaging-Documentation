---
title: Resize SVG Images Natively with Aspose.Imaging
linktitle: SVG Native Resize
type: docs
weight: 30
url: /net/svg-native-resize/
description: Demonstrates how to resize an SVG image and save it as PNG using Aspose.Imaging for .NET.
keywords: svg resize c#
---

# Resize SVG Images Natively

## Introduction
This example shows how to load an SVG file, resize it using native dimensions, and export the result as a PNG image. Use it when you need to programmatically adjust vector graphics size while preserving quality.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- An SVG file (e.g., `aspose_logo.svg`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder that contains the sample SVG file.  
2. Load the SVG image with `Image.Load` and cast it to `SvgImage`.  
3. Call `Resize` on the `SvgImage` instance, specifying the new width and height.  
4. Save the resized image as PNG using `PngOptions` with `SvgRasterizationOptions` for proper rasterization.  

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "dcd3bea58f9a8602f6434d95d72aef7a" "SvgNativeResize.cs" >}}

## See Also
- Converting SVG to other raster formats
- Working with vector rasterization options in Aspose.Imaging
- Resizing bitmap images with Aspose.Imaging for .NET
