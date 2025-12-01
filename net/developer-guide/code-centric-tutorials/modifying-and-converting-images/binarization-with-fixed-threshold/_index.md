---
title: Binarize an Image Using a Fixed Threshold
linktitle: Binarization with Fixed Threshold
type: docs
weight: 30
url: /net/binarization-with-fixed-threshold/
description: Demonstrates how to binarize an image using a fixed threshold with Aspose.Imaging for .NET.
keywords: binarize threshold c#
---

# Binarize an Image Using a Fixed Threshold

## Introduction
This example shows how to convert a raster image to a binary (black‑and‑white) representation by applying a predefined fixed threshold. Use it when you need a simple, fast way to create high‑contrast images for OCR, document scanning, or visual effects.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input image file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. **Load the source image** using `Image.Load`.
2. **Cast the image to `RasterCachedImage`** to work with raster‑specific operations.
3. **Ensure the image is cached** by checking `IsCached` and calling `CacheData` if necessary.
4. **Apply the fixed threshold** with `BinarizeFixed(thresholdValue)`, where `thresholdValue` is an integer between 0 and 255.
5. **Save the resulting binary image** to a new file.

## Code Example
The following snippet contains the complete runnable code for this scenario:

{{< gist "aspose-imaging-gists" "5ad52a4d7d6d5df55cb1bcc7e17deaa9" "BinarizationWithFixedThreshold.cs" >}}

## See Also
- [Converting Images to Grayscale](/net/converting-to-grayscale/)
- [Applying Adaptive Threshold Binarization](/net/adaptive-threshold-binarization/)
- [Working with Raster Cached Images](/net/raster-cached-image/)
