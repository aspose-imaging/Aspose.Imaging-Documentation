---
title: Export Image to PSD Format
linktitle: Export Image to PSD
type: docs
weight: 30
url: /net/export-image-to-psd/
description: Demonstrates how to export a bitmap image to PSD format using Aspose.Imaging for .NET.
keywords: psd export c#
---

# Export Image to PSD Format

## Introduction
This example shows how to load a bitmap image and save it as a Photoshop Document (PSD) using Aspose.Imaging for .NET. It is useful when you need to convert raster images to PSD for further editing in Photoshop or compatible software.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample bitmap file (`sample.bmp`) placed in the data directory

## Step-by-step Guide
1. **Prepare the data directory** – Determine the folder that contains the input bitmap file.
2. **Load the image** – Use `Image.Load` to read the bitmap into an `Image` object.
3. **Configure PSD options** – Create a `PsdOptions` instance and set properties such as `ColorMode`, `CompressionMethod`, and `Version`.
4. **Save as PSD** – Call `image.Save` with the target file name and the configured `PsdOptions`.
5. **Dispose resources** – Ensure the image object is disposed after saving to release file handles.

## Code Example
The following code demonstrates the export process:

{{< gist "aspose-imaging-gists" "6d6b95ddb9da89ca947752715c117d3b" "ExportImageToPSD.cs" >}}

## See Also
- Converting an image to PNG format
- Changing image color mode
- Saving images in different file formats
