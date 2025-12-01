---
title: Convert a PNG Image to 1‑Bit Color Depth
linktitle: Convert to 1‑Bit PNG
type: docs
weight: 20
url: /net/convert-to-1bit-png/
description: Demonstrates how to convert a PNG image to a 1‑bit (monochrome) PNG using Aspose.Imaging for .NET.
keywords: png, 1‑bit, convert c#
---

# Convert a PNG Image to 1‑Bit Color Depth

## Introduction
This example shows how to load a PNG file, adjust its bit depth to 1‑bit (monochrome), and save it as a new PNG using Aspose.Imaging for .NET. It is useful when you need to reduce file size or prepare images for environments that require only black‑and‑white pixels.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library installed
- A sample PNG file (e.g., `00020.png`) placed in the data directory used by the examples

## Step-by-step Guide
1. **Load the source image** – Use `Image.Load` with appropriate `LoadOptions` to read the PNG file.
2. **Determine bit depth** – Inspect the image’s `BitsPerPixel` to decide the target bit depth (1, 8, or 24).
3. **Create export options** – For PNG, configure a `PngOptions` instance, setting `BitDepth` to `1` and `ColorType` to `Grayscale` when the source depth is ≤ 8.
4. **Set additional options** – Optionally adjust `BufferSizeHint` and `ResolutionSettings` for performance and output quality.
5. **Save the converted image** – Call `image.Save` with the output file path and the prepared `PngOptions`.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "2ec84408c15966053affba007d442ba8" "ConvertTo1BitPng.cs" >}}

## See Also
- **Converting Images to Different Formats** – Learn how to convert between JPEG, PNG, and TIFF using Aspose.Imaging.
- **Changing Image Resolution** – Adjust DPI settings while saving images.
- **Working with Color Palettes** – Create custom palettes for indexed PNG and TIFF files.
