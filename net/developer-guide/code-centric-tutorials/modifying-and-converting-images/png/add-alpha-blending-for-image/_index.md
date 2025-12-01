---
title: Adding Alpha Blending to a PNG Image with Aspose.Imaging for .NET
linktitle: Add Alpha Blending (PNG)
type: docs
weight: 30
url: /net/add-alpha-blending-for-image/
description: Demonstrates how to blend an overlay image onto a PNG background using alpha blending.
keywords: alpha blending png c#
---

# Add Alpha Blending to a PNG Image

## Introduction
This example shows how to overlay one PNG image onto another using alpha blending with Aspose.Imaging for .NET. Use it when you need to combine images while preserving transparency.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- Sample PNG files: `image0.png` (background) and `aspose_logo.png` (overlay)

## Step-by-step Guide
1. Load the background PNG as a `RasterImage`.
2. Load the overlay PNG as a `RasterImage`.
3. Calculate the center point of the background where the overlay will be placed.
4. Call `Blend` on the background image, passing the overlay, its bounds, and an alpha value (e.g., 127 for 50% opacity).
5. Save the blended result to a new PNG file with `PngOptions` set to `TruecolorWithAlpha`.
6. Optionally delete the output file after verification.

## Code Example
Below is the full source code for the example:

{{< gist "aspose-imaging-gists" "f102f1a79c839ef49cd61538aee61896" "AddAlphaBlendingForImage.cs" >}}

## See Also
- Applying Watermarks to Images (C#)
- Adjusting Image Transparency with Aspose.Imaging
- Converting Image Formats Using Aspose.Imaging for .NET
