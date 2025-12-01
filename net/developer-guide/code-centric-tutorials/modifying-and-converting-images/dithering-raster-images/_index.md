---
title: Applying Dithering to Raster Images with Aspose.Imaging for .NET
linktitle: Dithering Raster Images
type: docs
weight: 30
url: /net/dithering-raster-images/
description: Demonstrates how to apply Floyd‑Steinberg dithering to a raster image and save the result.
keywords: dithering, raster, c#
---

# Applying Dithering to Raster Images

## Introduction
This example shows how to use Aspose.Imaging for .NET to perform Floyd‑Steinberg dithering on a raster image. It is useful when you need to reduce color depth while preserving visual detail, such as preparing images for limited‑color displays or certain printing workflows.

## Prerequisites
- .NET 6.0 or later (compatible with the Aspose.Imaging library)
- Aspose.Imaging for .NET library installed via NuGet
- Input image file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the directory containing the source image.
2. Load the source image as a `JpegImage` using `Image.Load`.
3. Call the `Dither` method on the image instance, specifying `DitheringMethod.ThresholdDithering` and the desired color depth (e.g., 4 bits).
4. Save the dithered image to a new file, such as a BMP, using the `Save` method.
5. Dispose of the image object to release resources (handled automatically with a `using` block).

## Code Example
The following code snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "2890e005f3d8b07752bc3ceb222d7cc8" "DitheringRasterImages.cs" >}}

## See Also
- [Converting Image Formats with Aspose.Imaging for .NET](#)
- [Applying Image Filters Using Aspose.Imaging for .NET](#)
- [Saving Images to Different File Types with Aspose.Imaging](#)
