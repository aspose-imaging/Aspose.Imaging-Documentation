---
title: Convert SVG to PNG Using Aspose.Imaging for .NET
linktitle: Convert SVG to PNG
type: docs
weight: 30
url: /net/svg-to-raster/
description: Demonstrates how to load an SVG file and export it as a PNG raster image with Aspose.Imaging for .NET.
keywords: svg png conversion c#
---

# Convert SVG to PNG

## Introduction
This example shows how to load an SVG image and save it as a PNG raster image using Aspose.Imaging for .NET. It is useful when you need to render vector graphics into a bitmap format for further processing or display.

## Prerequisites
- .NET 6.0 or later (compatible with your project)
- Aspose.Imaging for .NET library installed via NuGet
- SVG source file (e.g., `aspose_logo.svg`) placed in the example data folder

## Step-by-step Guide
1. **Prepare the environment** – Ensure the Aspose.Imaging package is referenced in your project.
2. **Set the data directory** – Define the path where the source SVG file is located.
3. **Load the SVG image** – Use `Image.Load` to read the SVG file as an `SvgImage` object.
4. **Configure PNG options** – Create an instance of `PngOptions` to specify PNG export settings.
5. **Save the raster image** – Call `image.Save` with the desired output path and PNG options.
6. **Verify the output** – The PNG file will be written to the specified location and can be opened with any image viewer.

## Code Example
The following snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "19774949b419ca960a759498dbba8ed1" "ConvertingSVGToRasterImages.cs" >}}

## See Also
- **Converting SVG to JPEG** – Learn how to export SVG images as JPEG files.
- **Batch converting images** – Process multiple images in a single operation.
- **Image format options** – Overview of available raster image format options in Aspose.Imaging.
