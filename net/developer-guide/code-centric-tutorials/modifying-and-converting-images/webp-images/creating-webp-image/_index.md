---
title: Creating a WebP Image with Aspose.Imaging for .NET
linktitle: Create WebP Image
type: docs
weight: 30
url: /net/creating-webp-image/
description: Demonstrates how to generate a lossless WebP image using Aspose.Imaging for .NET.
keywords: webp image c#
---

# Create a WebP Image

## Introduction
This example shows how to create a lossless WebP image from scratch using Aspose.Imaging for .NET. It is useful when you need to generate WebP graphics programmatically, such as for web delivery or image processing pipelines.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library installed
- No external image files are required; the example generates the image in memory

## Step-by-step Guide
1. **Create WebP options** – Instantiate `WebPOptions` and configure properties like `Lossless`.
2. **Set the output source** – Use `FileCreateSource` to define the destination file path.
3. **Create the image** – Call `Image.Create` with the `WebPOptions` and desired dimensions.
4. **Save the image** – Invoke `image.Save()` to write the WebP file to disk.
5. **Dispose resources** – The `using` statement ensures the image object is properly released.

## Code Example
The following code demonstrates the entire process:

{{< gist "aspose-imaging-gists" "3d4d86cf81f87a1fe22029f7582696a5" "CreatingWebPImage.cs" >}}

## See Also
- Converting an existing image to WebP format
- Optimizing WebP images for web performance
- Working with other image formats using Aspose.Imaging for .NET
