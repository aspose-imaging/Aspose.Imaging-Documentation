---
title: Blur an Image using Aspose.Imaging for .NET
linktitle: Blur an Image
type: docs
weight: 30
url: /net/blur-an-image/
description: Applies a Gaussian blur filter to an image and saves the result.
keywords: blur image c#
---

# Blur an Image

## Introduction
This example demonstrates how to apply a Gaussian blur filter to an image using Aspose.Imaging for .NET. Use it when you need to soften visual details or create a blurred effect for graphics and UI assets.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input image file (e.g., `asposelogo.gif`) placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the example data directory that contains the source image.  
2. Load the source image with `Image.Load`.  
3. Cast the loaded image to `RasterImage` to access raster‑specific operations.  
4. Create a `GaussianBlurFilterOptions` instance specifying the blur radius and sigma.  
5. Call `RasterImage.Filter`, passing the image bounds and the blur options.  
6. Save the processed image to a new file (e.g., `BlurAnImage_out.gif`).  

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "f736377df882ea2e5388fbac04e06f3b" "BlurAnImage.cs" >}}

## See Also
- Applying other image filters with Aspose.Imaging  
- Converting image formats using Aspose.Imaging  
- Saving images to different file types in .NET
