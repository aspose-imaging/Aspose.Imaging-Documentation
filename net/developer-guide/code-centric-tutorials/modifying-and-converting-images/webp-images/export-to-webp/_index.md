---
title: Export an Image to WebP Format using Aspose.Imaging for .NET
linktitle: Export to WebP
type: docs
weight: 30
url: /net/export-to-webp/
description: Demonstrates how to export a bitmap image to WebP format with adjustable quality.
keywords: webp export c#
---

# Export an Image to WebP

## Introduction
This example shows how to convert a BMP image to the WebP format using Aspose.Imaging for .NET. It demonstrates setting WebP-specific options such as quality and lossless compression, making it useful when you need lightweight images for web delivery.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample BMP image file (e.g., `SampleImage1.bmp`) placed in the example data folder

## Step-by-step Guide
1. **Prepare the input path** – Retrieve the directory containing the source BMP image.
2. **Load the source image** – Use `Image.Load` to read the BMP file into an `Image` object.
3. **Configure WebP options** – Create a `WebPOptions` instance and set properties such as `Quality` and `Lossless`.
4. **Save the image as WebP** – Call the `Save` method on the loaded image, providing the output filename and the configured `WebPOptions`.
5. **Verify the output** – The resulting file (`ExportToWebP_out.webp`) will be generated in the same folder.

## Code Example
The following code illustrates the complete process:

{{< gist "aspose-imaging-gists" "a0cd791be80598432be50ecdb85a04c8" "ExportToWebP.cs" >}}

## See Also
- Converting images to PNG format
- Working with WebP options for advanced encoding
- Saving images in different formats using Aspose.Imaging for .NET
