---
title: Adjust Image Brightness
linktitle: Adjust Brightness
type: docs
weight: 30
url: /net/adjust-brightness/
description: Demonstrates how to adjust the brightness of an image using Aspose.Imaging for .NET.
keywords: brightness, image processing, c#
---

# Adjust Image Brightness

## Introduction
This example shows how to increase the brightness of an image programmatically with Aspose.Imaging for .NET. It is useful when you need to enhance the visual appearance of photographs or graphics without altering other image properties.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An input JPEG image (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder that contains the source image.
2. Load the image using `Image.Load`.
3. Cast the loaded `Image` instance to `RasterImage` to access raster‑specific operations.
4. Ensure the raster data is cached for optimal performance with `RasterImage.CacheData`.
5. Call `RasterImage.AdjustBrightness` and specify the desired brightness level (0‑100).
6. Configure `TiffOptions` (or another format’s options) for the output file.
7. Save the modified image to a new file, for example `AdjustBrightness_out.tiff`.

## Code Example
The following code snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "391daab4adf0f30b99806908c3cfc061" "AdjustBrightness.cs" >}}

## See Also
- **Adjust Contrast** – Learn how to modify image contrast programmatically.  
- **Rotate Image** – Example for rotating images using Aspose.Imaging.  
- **Convert Image Format** – Guide on converting images between different file formats.
