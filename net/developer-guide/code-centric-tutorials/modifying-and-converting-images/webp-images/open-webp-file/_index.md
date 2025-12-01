---
title: Open WebP File and Modify Image
linktitle: Open WebP File
type: docs
weight: 30
url: /net/open-webp-file/
description: Open a WebP image, resize, crop, rotate, and save using Aspose.Imaging for .NET.
keywords: webp image c#
---

# Open WebP File and Modify Image

## Introduction
This example demonstrates how to load a WebP image, apply several transformations such as resizing, cropping, and rotating, and then save the modified image. Use it when you need to programmatically process WebP files in a .NET application.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library installed
- Sample WebP file (`Animation1.webp`) placed in the example data directory

## Step-by-step Guide
1. Retrieve the path to the folder containing the sample WebP image.
2. Load the WebP image using `Image.Load`.
3. Apply a high‑quality resize to the desired dimensions.
4. Crop a region of interest from the resized image.
5. Rotate and flip the image as required.
6. Save the transformed image to a memory stream.
7. Write the memory stream contents to a new WebP file on disk.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "195a7b66bf97d3430e4835e907fa291a" "OpenWebPFile.cs" >}}

## See Also
- Converting WebP images to other formats
- Resizing and cropping images with Aspose.Imaging
- Working with animated WebP files in .NET
