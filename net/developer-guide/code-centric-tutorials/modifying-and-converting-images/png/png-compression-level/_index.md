---
title: Control PNG Compression Level with Aspose.Imaging for .NET
linktitle: PNG Compression Level
type: docs
weight: 30
url: /net/png-compression-level/
description: Demonstrates how to set different PNG compression levels using Aspose.Imaging for .NET.
keywords: png compression c# aspnet
---

# Set PNG Compression Level

## Introduction
This example shows how to adjust the compression level of PNG images when saving them with Aspose.Imaging for .NET. Use it when you need to balance image quality against file size or optimize storage.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A PNG source file (e.g., `aspose_logo.png`) placed in the data directory used by the example

## Step-by-step Guide
1. Locate the directory containing the source PNG image.  
2. Load the image using `Image.Load`.  
3. Iterate through the desired compression levels (0 – 10).  
4. For each level, create a `PngOptions` object and set its `PngCompressionLevel` property.  
5. Save the image with the current options to a temporary file.  
6. Optionally delete the temporary file after verification.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "9a8736a9e25a6adb2c67d9716d5c4713" "PngCompressionLevelExample.cs" >}}

## See Also
- [Changing Image Format with Aspose.Imaging for .NET](#)
- [Optimizing JPEG Quality Settings](#)
