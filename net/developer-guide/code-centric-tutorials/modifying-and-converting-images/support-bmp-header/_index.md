---
title: Support BMP Header
linktitle: Support BMP Header
type: docs
weight: 30
url: /net/support-bmp-header/
description: Demonstrates how to load a BMP image and save it as PNG while preserving the BMP header using Aspose.Imaging for .NET.
keywords: bmp header, convert bmp png, c#
---

# Convert BMP Image to PNG While Supporting Header

## Introduction
This example shows how to load a BMP file and save it as a PNG image using Aspose.Imaging for .NET. It is useful when you need to convert BMP images without losing header information.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET
- A BMP source file (e.g., `source.bmp`) and write permissions for the output PNG file

## Step-by-step Guide
1. **Obtain the data directory** – Retrieve the folder that contains the input BMP file.
2. **Load the BMP image** – Use `Image.Load` to read the source BMP file.
3. **Create PNG options** – Instantiate `PngOptions` to specify PNG format settings.
4. **Save the image as PNG** – Call `image.Save` with the desired output path and PNG options.
5. **Dispose resources** – The `using` statement ensures the image object is released properly.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b3c12ae8b32d444c0fce358cbf06a118" "SupportBMPHeader.cs" >}}

## See Also
- Convert BMP to JPEG
- Modify Image Metadata
- Save Image in Different Formats
