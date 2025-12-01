---
title: Remove Watermark from PNG Images using Aspose.Imaging
linktitle: Remove Watermark
type: docs
weight: 30
url: /net/remove-watermark-filter/
description: Demonstrates how to remove a watermark from a PNG image using Aspose.Imaging for .NET.
keywords: watermark removal, png, c#
---

# Remove Watermark from PNG Images

## Introduction
This example shows how to programmatically erase a watermark from a PNG image by defining a mask and using Aspose.Imaging's content‑aware fill functionality. Use it when you need to clean up images that contain unwanted logos or overlays.

## Prerequisites
- .NET 6.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- A PNG file named **ball.png** placed in the data directory used by the example

## Step-by-step Guide
1. Load the source PNG image with `Image.Load`.
2. Create a `GraphicsPath` mask that outlines the watermark area (e.g., an ellipse).
3. Configure `ContentAwareFillWatermarkOptions` and set the desired painting attempts.
4. Call `WatermarkRemover.PaintOver` to generate a cleaned image.
5. Save the resulting image and optionally delete the intermediate file.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "638460790f837395948e1a520d1a0c26" "RemoveWatermarkFilter.cs" >}}

## See Also
- Applying Watermarks to Images
- Content‑Aware Fill with Magic Wand
- Working with PNG Images in Aspose.Imaging
