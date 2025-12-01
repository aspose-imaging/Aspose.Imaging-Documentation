---
title: Applying Motion Wiener Filter
linktitle: Motion Wiener Filter
type: docs
weight: 30
url: /net/applying-motion-wiener-filter/
description: Demonstrates how to apply a Motion Wiener filter to a raster image using Aspose.Imaging for .NET.
keywords: motion wiener filter, image processing, c#
---

# Applying Motion Wiener Filter

## Introduction
This example shows how to apply a Motion Wiener filter—a motion‑blur reducing filter—to a raster image. It is useful when you need to enhance GIF or other raster images that suffer from motion blur or noise.

## Prerequisites
- .NET 6.0 or later (any supported .NET runtime)
- Aspose.Imaging for .NET library
- An input GIF image (e.g., `asposelogo.gif`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the example data directory.  
2. Load the source image using `Image.Load`.  
3. Cast the loaded image to `RasterImage`.  
4. Create a `MotionWienerFilterOptions` object and configure length, smooth value, angle, and grayscale settings.  
5. Call the `Filter` method on the raster image, passing the image bounds and filter options.  
6. Save the filtered image to a new file (e.g., `ApplyingMotionWienerFilter_out.gif`).  

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "c859d4b2ea3ba737029d56953dee7f23" "ApplyingMotionWienerFilter.cs" >}}

## See Also
- **Applying Gaussian Blur Filter** – Learn how to soften images using a Gaussian blur.  
- **Saving Images in Different Formats** – Convert and save images to various file types such as PNG, JPEG, and BMP.  
- **Working with Raster Images** – Explore other raster‑image operations like pixel manipulation and color conversion.
