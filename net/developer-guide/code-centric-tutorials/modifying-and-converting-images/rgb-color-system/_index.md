---
title: Convert RGB TIFF Image to CMYK Using Aspose.Imaging
linktitle: RGB to CMYK
type: docs
weight: 30
url: /net/rgb-color-system/
description: Demonstrates how to convert an RGB TIFF image to CMYK using Aspose.Imaging for .NET.
keywords: tiff conversion c#
---

# Convert RGB TIFF Image to CMYK Using Aspose.Imaging

## Introduction
This example shows how to change the color space of a TIFF image from RGB to CMYK using Aspose.Imaging for .NET. It is useful when you need to prepare images for printing workflows that require CMYK color profiles.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library installed
- A sample RGB TIFF file (e.g., `testTileDeflate.tif`) available in the working directory

## Step-by-step Guide
1. **Set up the source and output file paths** – define the location of the original RGB TIFF and the desired CMYK output file.  
2. **Create `TiffOptions` with CMYK format** – instantiate `TiffOptions` using `TiffExpectedFormat.TiffLzwCmyk` to specify the CMYK color space.  
3. **Load the image** – use `Image.Load` to read the source TIFF into an `Image` object.  
4. **Save the image with the new options** – call `image.Save(outputPath, options)` to write the file as a CMYK TIFF.  

## Code Example
The following code shows how to perform the conversion:

{{< gist "aspose-imaging-gists" "d2c1588be25d314c4ff1149e68b8a835" "RGBColorSytem.cs" >}}

## See Also
- **Saving images in different formats** – Learn how to export images to PNG, JPEG, BMP, and other formats.  
- **Working with TIFF options** – Explore additional TIFF settings such as compression and resolution.  
- **Changing color space of images** – Understand how to convert between RGB, CMYK, and grayscale using Aspose.Imaging.
