---
title: Apply Manual Image Masking with Aspose.Imaging for .NET
linktitle: Manual Image Masking
type: docs
weight: 30
url: /net/manual-image-masking/
description: Demonstrates how to apply a manual mask to an image using Aspose.Imaging for .NET.
keywords: manual mask c# image masking
---

# Apply Manual Image Masking with Aspose.Imaging for .NET

## Introduction
This example shows how to create and apply a custom manual mask to a raster image using Aspose.Imaging for .NET. Use it when you need precise control over which parts of an image are retained or removed.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A PNG image file to serve as the source (e.g., *Colored by Faith_small.png*)

## Step-by-step Guide
1. **Prepare the source image path** – locate the PNG file you want to mask.  
2. **Create a `GraphicsPath`** – define the mask geometry using shapes such as ellipses, rectangles, polygons, and pies.  
3. **Load the image** – use `Image.Load` to read the source file as a `RasterImage`.  
4. **Configure `MaskingOptions`** – set the segmentation method to `Manual` and assign the `GraphicsPath` to `ManualMaskingArgs`.  
5. **Perform masking** – instantiate `ImageMasking` and call `Decompose` with the configured options.  
6. **Save the result** – retrieve the masked image from the result set and save it to the desired output path.

## Code Example
The complete source code is shown below:

{{< gist "aspose-imaging-gists" "a85540359d524552840b76af30f1e208" "ManualImageMasking.cs" >}}

## See Also
- **Applying Automatic Image Masking** – learn how to let Aspose.Imaging detect mask regions automatically.  
- **Converting Image Formats** – explore converting between PNG, JPEG, and other formats using Aspose.Imaging.  
- **Working with Image Layers** – understand how to manipulate image layers for advanced compositing.
