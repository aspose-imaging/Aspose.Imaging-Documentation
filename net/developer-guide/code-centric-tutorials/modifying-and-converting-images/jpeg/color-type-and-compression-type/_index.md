---
title: Set JPEG Color Type and Compression Type with Aspose.Imaging for .NET
linktitle: JPEG Color Type & Compression
type: docs
weight: 30
url: /net/color-type-and-compression-type/
description: Demonstrates how to change JPEG color mode and compression type using Aspose.Imaging for .NET.
keywords: jpeg color type c#
---

# Set JPEG Color Type and Compression Type

## Introduction
This example shows how to modify the color mode and compression type of a JPEG image using Aspose.Imaging for .NET. It is useful when you need to create grayscale or progressive JPEG files from existing images.

## Prerequisites
- .NET 5.0 or later (the sample was built with .NET 9.0)
- Aspose.Imaging for .NET library
- An input image file (e.g., a GIF) to be converted to JPEG

## Step-by-step Guide
1. **Prepare the source image** – Locate the image you want to convert (for example, `ColorGif.gif`).
2. **Create a `JpegOptions` instance** – Set the desired `ColorType` (e.g., `Grayscale`) and `CompressionType` (e.g., `Progressive`).
3. **Load the source image** using `Image.Load`.
4. **Save the image** with the configured `JpegOptions` to the target path.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "ace54e60f2543e7db773cfc34b4ffcdd" "ColorTypeAndCompressionType.cs" >}}

## See Also
- [Adjust JPEG Quality Settings](#)
- [Convert Images to Different Formats](#)
- [Working with JPEG Options in Aspose.Imaging](#)
