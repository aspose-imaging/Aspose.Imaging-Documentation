---
title: Add Watermark to Image
linktitle: Add Watermark
type: docs
weight: 30
url: /net/add-watermark-to-image/
description: Demonstrates how to add a text watermark to an image using Aspose.Imaging for .NET.
keywords: watermark image c#
---

# Add Watermark to Image

## Introduction
This example shows how to overlay a text watermark onto an existing bitmap image using Aspose.Imaging for .NET. It is useful when you need to brand images or embed copyright information programmatically.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A source bitmap file named `WaterMark.bmp` placed in the example data folder

## Step-by-step Guide
1. Load the source image with `Image.Load`.
2. Create a `Graphics` object linked to the loaded image.
3. Define a `Font` describing the watermark text style.
4. Create a `SolidBrush` and set its color and opacity.
5. Use `Graphics.DrawString` to draw the watermark text at the desired location.
6. Save the modified image to a new file (e.g., `AddWatermarkToImage_out.bmp`).

## Code Example
The following snippet contains the complete source code for the example:

{{< gist "aspose-imaging-gists" "5053765dc0930f6499a740ada056a96c" "AddWatermarkToImage.cs" >}}

## See Also
- **Rotate Image** – Learn how to rotate images by arbitrary angles.
- **Resize Image** – Understand image scaling and resizing techniques.
- **Add Text to Image** – Explore adding generic text annotations without a watermark.
