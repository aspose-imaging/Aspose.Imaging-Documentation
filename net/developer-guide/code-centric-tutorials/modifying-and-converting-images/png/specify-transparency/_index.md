---
title: Specify Transparency for PNG Images
linktitle: Specify Transparency
type: docs
weight: 30
url: /net/specify-transparency/
description: Demonstrates how to set a transparent color when creating a PNG image with Aspose.Imaging for .NET.
keywords: png transparency c#
---

# Specify Transparency for PNG Images

## Introduction
This example shows how to create a PNG image with a specific transparent color using Aspose.Imaging for .NET. It is useful when you need to render a particular color as fully transparent in the resulting PNG.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A source BMP or PNG image file (e.g., `aspose_logo.png`) placed in the example data folder

## Step-by-step Guide
1. Load the source image into a `RasterImage` to obtain its pixel data.
2. Create a new `PngImage` with the desired dimensions and set `PngColorType.TruecolorWithAlpha`.
3. Save the loaded pixel data into the new PNG image.
4. Assign the `TransparentColor` property (e.g., `Color.Black`) to specify which color should become transparent.
5. Set `HasTransparentColor` to `true` and save the PNG image to disk.

## Code Example
The following code demonstrates how to specify a transparent color for a PNG image:

{{< gist "aspose-imaging-gists" "45a2de98ee07b655953f1415a250ff44" "SpecifyTransparency.cs" >}}

## See Also
- Converting BMP to PNG with Aspose.Imaging
- Working with PNG color types and alpha channels
- Applying image filters using Aspose.Imaging for .NET
