---
title: Apply Gauss‑Wiener Filter to a Colored Image
linktitle: Gauss‑Wiener Filter
type: docs
weight: 30
url: /net/apply-gauss-wiener-filter-colored-image/
description: Demonstrates how to apply the Gauss‑Wiener filter to a colored image using Aspose.Imaging for .NET.
keywords: gauss wiener filter c#
---

# Apply Gauss‑Wiener Filter to a Colored Image

## Introduction
This example shows how to use the Gauss‑Wiener filter to enhance a colored image. It is useful when you need to reduce noise while preserving edges in GIF or other raster images.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample image file `asposelogo.gif` placed in the designated data directory

## Step-by-step Guide
1. Locate the data directory that contains the source image.
2. Load the image using `Image.Load`.
3. Cast the loaded image to a `RasterImage`.
4. Create a `GaussWienerFilterOptions` instance, specifying radius and smoothness values.
5. Optionally adjust additional properties such as `Brightness`.
6. Apply the filter to the raster image with `RasterImage.Filter`.
7. Save the processed image to a new file.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "dbf48a70afb09037416f8aa3905e092a" "ApplyGaussWienerFilterForColoredImage.cs" >}}

## See Also
- **Applying Other Image Filters** – Learn how to apply different filters like median or Gaussian blur.
- **Converting Image Formats** – Example of converting images between supported formats.
- **Working with Raster Images** – Overview of raster image manipulation using Aspose.Imaging.
