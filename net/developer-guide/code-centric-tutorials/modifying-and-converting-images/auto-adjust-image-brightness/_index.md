---
title: Automatically Adjust Image Brightness
linktitle: Auto Adjust Brightness
type: docs
weight: 30
url: /net/auto-adjust-image-brightness/
description: Demonstrates how to automatically adjust image brightness using Aspose.Imaging for .NET.
keywords: brightness image c#
---

# Automatically Adjust Image Brightness

## Introduction
This example shows how to automatically normalize the histogram of an image and then adjust its contrast, effectively improving the perceived brightness. Use it when you need a quick way to enhance image quality without manual tuning.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample PNG image (e.g., `sample.png`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder containing the sample image.
2. Load the PNG image as a `RasterImage`.
3. Call `NormalizeHistogram()` to automatically balance brightness and contrast.
4. Save the normalized image to verify the changes.
5. Adjust the contrast further with `AdjustContrast(30)` (or another value) to fine‑tune brightness.
6. Save the final image and clean up any temporary files.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "1bf5ed5a5e59d1e8fbbec650770e449d" "AutoAdjustImageBrightness.cs" >}}

## See Also
- [Adjust Image Contrast](../adjust-image-contrast/)
- [Histogram Normalization Overview](../histogram-normalization/)
- [Working with Raster Images in Aspose.Imaging](../raster-images/)
