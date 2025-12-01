---
title: Convert SVG to BMP with Aspose.Imaging for .NET
linktitle: SVG to BMP conversion
type: docs
weight: 30
url: /net/svg-to-bmp-conversion/
description: Demonstrates how to convert an SVG image to BMP format using Aspose.Imaging for .NET.
keywords: svg bmp conversion c#
---

# Convert SVG to BMP with Aspose.Imaging for .NET

## Introduction
This example shows how to load an SVG file and save it as a BMP image using Aspose.Imaging for .NET. It is useful when you need rasterized bitmap output from vector graphics for compatibility with legacy systems or image processing pipelines.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library installed
- An SVG file (e.g., `test.svg`) placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the SVG source file.  
2. Load the SVG image using `Image.Load`.  
3. Create a `BmpOptions` instance to specify BMP output settings.  
4. Configure `SvgRasterizationOptions` (e.g., page width and height) and assign it to the `VectorRasterizationOptions` property of the BMP options.  
5. Call `image.Save` with the target BMP file name and the configured options.  
6. Verify that the BMP file is created in the output location.

## Code Example
The following code demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "d1b68d25fd7f3a668c2a07c05ee717ab" "SVGToBMPConversion.cs" >}}

## See Also
- Converting SVG to PNG with Aspose.Imaging for .NET  
- Rasterizing vector images using `SvgRasterizationOptions`  
- Working with image formats: loading, editing, and saving in Aspose.Imaging
