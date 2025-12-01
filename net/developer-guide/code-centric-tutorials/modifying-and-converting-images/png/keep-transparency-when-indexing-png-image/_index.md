---
title: Keep Transparency When Indexing PNG Image
linktitle: Keep Transparency PNG
type: docs
weight: 30
url: /net/keep-transparency-when-indexing-png-image/
description: Demonstrates how to preserve transparency while indexing a PNG image using Aspose.Imaging for .NET.
keywords: png transparency c#
---

# Keep Transparency When Indexing PNG Image

## Introduction
This example shows how to retain the transparency information when converting a PNG image to an indexed‑color format. Use it when you need a smaller PNG file without losing its alpha channel.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A source PNG file (e.g., `template.png`) placed in the example data folder

## Step-by-step Guide
1. Load the source PNG image as a `RasterImage`.
2. Create a `PngOptions` object and set:
   - `CompressionLevel` to control file size.
   - `ColorType` to `IndexedColor`.
   - `Palette` using `ColorPaletteHelper.GetCloseTransparentImagePalette` to generate a palette that includes transparent colors.
   - `FilterType` as needed (e.g., `Avg`).
3. Save the image with the configured options, producing an indexed PNG that keeps transparency.
4. (Optional) Delete the generated file after verification.

## Code Example
The following code demonstrates the entire process:

{{< gist "aspose-imaging-gists" "a7b01d828c3bfdeaa5e1f21123d36d87" "KeepTransparencyWhenIndexingPngImage.cs" >}}

## See Also
- [Converting PNG to Different Color Types](#)
- [Using ColorPaletteHelper for Custom Palettes](#)
- [Optimizing PNG Compression Settings](#)
