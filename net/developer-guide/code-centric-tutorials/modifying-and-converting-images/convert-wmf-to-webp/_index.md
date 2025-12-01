---
title: Convert WMF to WebP Using Aspose.Imaging for .NET
linktitle: Convert WMF to WebP
type: docs
weight: 30
url: /net/convert-wmf-to-webp/
description: Demonstrates how to convert a WMF image to WebP format with Aspose.Imaging for .NET.
keywords: wmf webp conversion
---

# Convert WMF to WebP

## Introduction
This example shows how to load a WMF (Windows Metafile) image and save it as a WebP image using Aspose.Imaging for .NET. Use it when you need to rasterize vector WMF files into modern WebP format with custom dimensions.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input WMF file (`input.wmf`) placed in the example data directory

## Step-by-step Guide
1. **Set up the data directory** – obtain the path where the input WMF file resides.  
2. **Load the WMF image** – use `Image.Load` to read the WMF file.  
3. **Calculate aspect ratio** – determine the scaling factor to keep the image proportions.  
4. **Configure rasterization options** – create a `WmfRasterizationOptions` object and set background color, page size, and margins.  
5. **Create WebP options** – instantiate `WebPOptions` and assign the rasterization options to `VectorRasterizationOptions`.  
6. **Save as WebP** – call `image.Save` with the output file name and the WebP options.

## Code Example
The following code demonstrates the conversion:

{{< gist "aspose-imaging-gists" "f46fd3e25162900670683da2d68253f4" "ConvertWMFToWebp.cs" >}}

## See Also
- [Convert WMF to PNG](/net/convert-wmf-to-png/)
- [Convert EMF to WebP](/net/convert-emf-to-webp/)
- [Rasterizing vector images with Aspose.Imaging](/net/rasterizing-vector-images/)
