---
title: Specify Bit Depth for PNG Images
linktitle: Specify Bit Depth
type: docs
weight: 30
url: /net/specify-bit-depth/
description: Demonstrates how to set the color type and bit depth when saving a PNG image with Aspose.Imaging for .NET.
keywords: png bitdepth c#
---

# Specify Bit Depth for PNG Images

## Introduction
This example shows how to change the color type and bit depth of a PNG image before saving it. It is useful when you need to reduce file size or conform to specific PNG specifications.

## Prerequisites
- .NET 6.0 or later (or any supported .NET version)
- Aspose.Imaging for .NET library
- A sample PNG file (e.g., `aspose_logo.png`) placed in the appropriate data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the source PNG file.  
2. Load the PNG image using `Image.Load`.  
3. Create a `PngOptions` instance.  
4. Set `ColorType` to the desired value (e.g., `PngColorType.Grayscale`).  
5. Set the corresponding `BitDepth` (e.g., `1` for 1‑bit grayscale).  
6. Save the image with the configured options to a new file.

## Code Example
The following code demonstrates the process:

{{< gist "aspose-imaging-gists" "9edce3e5753a46104874dea567a3cfff" "SpecifyBitDepth.cs" >}}

## See Also
- [Converting PNG to JPEG with Aspose.Imaging for .NET](https://docs.aspose.com/imaging/net/convert-png-to-jpeg/)
- [Changing Image Color Depth Using Aspose.Imaging](https://docs.aspose.com/imaging/net/change-image-color-depth/)
- [Working with PNG Options in Aspose.Imaging](https://docs.aspose.com/imaging/net/png-options/)
