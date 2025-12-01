---
title: Using Image Scoped Fonts with Aspose.Imaging for .NET
linktitle: Image Scoped Fonts
type: docs
weight: 30
url: /net/image-scoped-fonts/
description: Demonstrates how to load images with custom font sources using Aspose.Imaging for .NET.
keywords: custom fonts, rasterization, c#
---

# Use Image Scoped Fonts to Load Images with Custom Fonts

## Introduction
This example shows how to work with images that rely on fonts not embedded in the file. By providing a custom font source, you can correctly render vector images such as EMF, SVG, WMF, and ODG. Use this approach when processing documents that reference external fonts.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A set of sample image files (e.g., *missing-font.emf*, *missing-font.svg*) and a folder containing the required font files

## Step-by-step Guide
1. **Prepare the data directory** – Locate the folder that contains the sample images and the custom fonts.
2. **Create `LoadOptions`** – Instantiate `Aspose.Imaging.LoadOptions` and add a custom font source via `AddCustomFontSource`, pointing to the fonts folder.
3. **Load each image** – Use `Image.Load` with the configured `LoadOptions` to open the vector file.
4. **Configure rasterization** – Retrieve default rasterization options, set `TextRenderingHint` and `SmoothingMode` to control how text is rendered.
5. **Save the rasterized image** – Export the processed image to PNG (or another raster format) using the prepared rasterization options.
6. **Clean up** – Delete any intermediate files if needed.

## Code Example
The following snippet contains the complete implementation of the steps described above.

{{< gist "aspose-imaging-gists" "4667aa3ca9c47a7bfdbe14398b836c84" "ImageScopedFonts.cs" >}}

## See Also
- **Working with Vector Images** – Learn how to rasterize other vector formats using Aspose.Imaging.  
- **Managing Fonts in Aspose.Imaging** – Explore additional ways to handle font embedding and substitution.  
- **Converting Images to Different Formats** – Convert rasterized images to JPEG, BMP, or TIFF.
