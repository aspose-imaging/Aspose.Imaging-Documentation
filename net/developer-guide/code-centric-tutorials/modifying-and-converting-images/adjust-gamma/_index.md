---
title: Adjust Image Gamma with Aspose.Imaging for .NET
linktitle: Adjust Gamma
type: docs
weight: 30
url: /net/adjust-gamma/
description: Adjust the gamma of an image and save it as a TIFF file using Aspose.Imaging for .NET.
keywords: adjust gamma image c#
---

# Adjust Image Gamma with Aspose.Imaging for .NET

## Introduction
This example demonstrates how to modify the gamma levels of a raster image and then save the result in TIFF format. Use it when you need to enhance image brightness or contrast by adjusting gamma values.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An input image file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Load the source image using `Image.Load`.
2. Cast the loaded image to `RasterImage`.
3. Ensure the raster image data is cached for optimal performance.
4. Call `AdjustGamma` with the desired gamma values for each channel.
5. Configure `TiffOptions` (bits per sample, photometric settings, etc.).
6. Save the modified raster image as a TIFF file using `RasterImage.Save`.

## Code Example
The following code snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "313a9e298e4ff7dfc9a2cd8e130a72b2" "AdjustGamma.cs" >}}

## See Also
- Adjusting image brightness with Aspose.Imaging
- Converting images between formats using Aspose.Imaging
- Caching raster image data for performance improvements
