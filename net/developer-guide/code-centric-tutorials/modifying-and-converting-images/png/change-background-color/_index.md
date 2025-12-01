---
title: Change Background Color in PNG Images
linktitle: Change Background Color
type: docs
weight: 30
url: /net/change-background-color/
description: Demonstrates how to replace a transparent background with white in a PNG image using Aspose.Imaging for .NET.
keywords: png background color c#
---

# Change Background Color in PNG Images

## Introduction
This example shows how to modify a PNG image by detecting its transparent background pixels and replacing them with white. Use it when you need to ensure a PNG image has an opaque background for downstream processing or display.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Input PNG file (e.g., `aspose_logo.png`) placed in the example data directory

## Step-by-step Guide
1. Load the source PNG image using `Image.Load`.
2. Cast the loaded image to `RasterImage` to access pixel data.
3. Retrieve the ARGB pixel array with `LoadArgb32Pixels`.
4. Iterate through the pixel array, compare each pixel to the image’s `TransparentColor`, and replace matching pixels with white (`Color.White`).
5. Write the modified pixel array back to the image using `SaveArgb32Pixels`.
6. Save the updated image to a new file (e.g., `ChangeBackgroundColor_out.jpg`).

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "c4c118bcc3fdcba56d26e07d0a857fb6" "ChangeBackgroundColor.cs" >}}

## See Also
- **Changing Image Format** – Convert PNG to JPEG or other formats using Aspose.Imaging.
- **Applying Image Effects** – Explore how to apply filters such as grayscale or sepia.
- **Working with Raster Images** – Learn more about pixel-level manipulation with `RasterImage`.
