---
title: Export WebP Image to Other Formats
linktitle: Export WebP to Other Formats
type: docs
weight: 30
url: /net/export-webp-to-other-image-formats/
description: Demonstrates how to load a WebP image and save it to another format using Aspose.Imaging for .NET.
keywords: webp convert c#
---

# Export WebP Image to Other Formats

## Introduction
This example shows how to load a WebP image with Aspose.Imaging for .NET and save it to a different format. It is useful when you need to convert WebP assets to more widely supported formats such as BMP, PNG, or JPEG.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A WebP image file (e.g., `asposelogo.webp`) placed in the example data directory

## Step-by-step Guide
1. **Determine the data directory** – Use `RunExamples.GetDataDir_WebPImages()` to obtain the path where the source WebP file resides.  
2. **Load the WebP image** – Call `Image.Load()` with the full path to the WebP file.  
3. **Save the image in the desired format** – Invoke `image.Save()` with the target file name and an appropriate options class (e.g., `BmpOptions` for BMP).  
4. **Optional console output** – Write messages before and after the conversion to track execution.

## Code Example
The following snippet implements the steps described above:

{{< gist "aspose-imaging-gists" "042d0fd6072bba62e8ddeb6fdb55c0bb" "ExportWebPToOtherImageFormats.cs" >}}

## See Also
- Converting WebP to PNG using Aspose.Imaging  
- Working with other image formats (BMP, JPEG, TIFF) in Aspose.Imaging  
- Basic image manipulation techniques with Aspose.Imaging for .NET
