---
title: Compress PNG Files with Different Compression Levels
linktitle: Compress PNG Files
type: docs
weight: 30
url: /net/compressing-files/
description: Demonstrates how to compress PNG images using various compression levels with Aspose.Imaging for .NET.
keywords: compress png c#
---

# Compress PNG Files with Different Compression Levels

## Introduction
This example shows how to load a PNG image and save multiple copies using different compression levels. It is useful when you need to balance file size and image quality for PNG assets.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample PNG image (e.g., `aspose_logo.png`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder containing the source PNG image.  
2. Load the PNG image using `Image.Load`.  
3. Iterate through compression levels from 0 to 9.  
4. For each level, create a `PngOptions` instance and set its `CompressionLevel` property.  
5. Save the image with the current compression level, naming the output file to reflect the level (e.g., `0_out.png`, `1_out.png`, … `9_out.png`).  

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "de1271a2dd80bf8214dcb38bf27a91a7" "CompressingFiles.cs" >}}

## See Also
- [Saving Images in Different Formats](#)
- [Optimizing Image Quality and File Size](#)
- [Working with PNG Options in Aspose.Imaging](#)
