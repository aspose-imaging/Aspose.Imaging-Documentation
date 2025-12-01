---
title: Convert WMF Metafile to SVG Using Aspose.Imaging for .NET
linktitle: Convert WMF to SVG
type: docs
weight: 30
url: /net/convert-wmf-meta-file-to-svg/
description: Demonstrates how to convert a WMF metafile to SVG format with Aspose.Imaging for .NET.
keywords: wmf svg conversion c#
---

# Convert WMF Metafile to SVG

## Introduction
This example shows how to load a WMF (Windows Metafile) image and convert it to an SVG (Scalable Vector Graphics) file using Aspose.Imaging for .NET. Use this when you need to preserve vector quality while switching to a web‑friendly SVG format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A WMF file named **input.wmf** placed in the example data directory

## Step-by-step Guide
1. **Get the data directory** – Locate the folder that contains the source WMF file.
2. **Load the WMF image** – Use `Image.Load` to read the WMF file into an `Image` object.
3. **Configure rasterization options** – Create a `WmfRasterizationOptions` instance and set `PageWidth` and `PageHeight` to match the original image dimensions.
4. **Save as SVG** – Call `image.Save` with an output path and an `SvgOptions` object that references the rasterization options.
5. **Dispose resources** – The `using` statement automatically releases the image resources.

## Code Example
The following code demonstrates the conversion process:

{{< gist "aspose-imaging-gists" "b9dacb192a5004f58a7eaa95db960d35" "ConvertWMFMetaFileToSVG.cs" >}}

## See Also
- [Converting BMP to PNG with Aspose.Imaging for .NET](#)
- [Applying Image Filters Using Aspose.Imaging for .NET](#)
