---
title: Binarize an Image Using Otsu Thresholding
linktitle: Binarization with Otsu Threshold
type: docs
weight: 30
url: /net/binarization-with-otsu-threshold/
description: Demonstrates how to binarize an image using Otsu thresholding with Aspose.Imaging for .NET.
keywords: binarize, otsu, c#
---

# Binarize an Image Using Otsu Thresholding

## Introduction
This example shows how to convert a color image into a binary (black‑and‑white) image using Otsu’s automatic thresholding algorithm. It is useful when you need to prepare images for OCR, document analysis, or any scenario where a clear binary representation is required.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Input image file (e.g., `aspose-logo.jpg`) placed in the example data directory

## Step-by-step Guide
1. Load the source image with `Image.Load`.
2. Cast the loaded image to `RasterCachedImage` to work with raster‑based operations.
3. Ensure the raster image is cached; call `CacheData` if necessary.
4. Apply Otsu thresholding by invoking `BinarizeOtsu()`.
5. Save the resulting binary image to a file (e.g., `BinarizationWithOtsuThreshold_out.jpg`).

## Code Example
The following code demonstrates the Otsu binarization process:

{{< gist "aspose-imaging-gists" "a3960aa5b8b2ce76c7f631d3d96b692b" "BinarizationWithOtsuThreshold.cs" >}}

## See Also
- Converting images to different formats with Aspose.Imaging
- Applying other image binarization techniques
- Working with raster‑cached images in Aspose.Imaging
