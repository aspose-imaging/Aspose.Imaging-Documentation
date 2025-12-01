---
title: Add a Diagonal Watermark to an Image
linktitle: Diagonal Watermark
type: docs
weight: 20
url: /net/add-diagonal-watermark-to-image/
description: Demonstrates how to add a rotated diagonal text watermark to an image using Aspose.Imaging for .NET.
keywords: watermark image c#
---

# Add a Diagonal Watermark to an Image

## Introduction
This example shows how to place a 45‑degree rotated text watermark across an image. Use it when you need to embed branding or copyright information that spans the image diagonally.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample TIFF image (`SampleTiff1.tiff`) placed in the example data folder

## Step-by-step Guide
1. Load the source image using `Image.Load`.
2. Create a `Graphics` object from the image to enable drawing.
3. Prepare the watermark text, font, and a `SolidBrush` with the desired color.
4. Build a transformation matrix:
   - Translate the matrix to the center of the image.
   - Rotate the matrix by -45 degrees.
5. Assign the matrix to `Graphics.Transform`.
6. Draw the string onto the image with `Graphics.DrawString`.
7. Save the resulting image, e.g., `AddDiagonalWatermarkToImage_out.jpg`.

## Code Example
The following snippet illustrates the complete process:

{{< gist "aspose-imaging-gists" "2525b20829867ec754dc425533715c99" "AddDiagonalWatermarkToImage.cs" >}}

## See Also
- Adding a text watermark to an image (horizontal)
- Adjusting watermark opacity and color
- Converting image formats with Aspose.Imaging for .NET
