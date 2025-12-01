---
title: "Apply Gauss‑Wiener Filter to an Image"
linktitle: "Gauss‑Wiener Filter"
type: docs
weight: 30
url: /net/apply-gauss-wiener-filter/
description: "Demonstrates how to apply a Gauss‑Wiener filter to a raster image using Aspose.Imaging for .NET."
keywords: "gauss wiener filter c#"
---

# Apply Gauss‑Wiener Filter to an Image

## Introduction
This example shows how to apply a Gauss‑Wiener filter to a raster image with Aspose.Imaging for .NET. Use it when you need to smooth noisy images while preserving edges.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample GIF image (e.g., `asposelogo.gif`) placed in the example data folder

## Step-by-step Guide
1. Load the source image using `Image.Load`.
2. Cast the loaded image to `RasterImage`.
3. Create a `GaussWienerFilterOptions` object, specifying radius and smoothness, and set `Grayscale` as needed.
4. Apply the filter to the raster image with `RasterImage.Filter`.
5. Save the filtered image to the desired output format.

## Code Example
Below is the complete code for the example:

{{< gist "aspose-imaging-gists" "050edd7089525aca2a44a6875a41abd4" "ApplyGaussWienerFilter.cs" >}}

## See Also
- [Applying Gaussian Blur Filter](/net/apply-gaussian-blur-filter/)
- [Converting Image Formats](/net/convert-image-format/)
- [Working with Raster Images](/net/raster-image-manipulation/)
