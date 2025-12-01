---
title: Compress SVG to SVGZ Using Aspose.Imaging
linktitle: Compress SVG
type: docs
weight: 30
url: /net/compressed-vector-formats/
description: Demonstrates how to compress an SVG image to SVGZ format using Aspose.Imaging for .NET.
keywords: compress svg c#
---

# Compress SVG to SVGZ Using Aspose.Imaging

## Introduction
This example shows how to load an SVG file, configure rasterization options, and save it as a compressed SVGZ file. Use it when you need smaller vector files for faster web delivery or reduced storage space.

## Prerequisites
- .NET 6.0 or later (compatible with the Aspose.Imaging for .NET library)
- Aspose.Imaging for .NET installed
- A sample SVG file (e.g., `Sample.svg`) placed in the data directory used by the examples

## Step-by-step Guide
1. Determine the path to the directory containing the source SVG file.  
2. Load the SVG image using `Image.Load`.  
3. Create an instance of `SvgRasterizationOptions` (or `VectorRasterizationOptions`) and set the desired page size based on the original image dimensions.  
4. Prepare `SvgOptions`, assign the rasterization options, and enable compression by setting `Compress = true`.  
5. Save the image to a new file with an `.svgz` extension using `image.Save`.  
6. Verify that the resulting file size is smaller than the original SVG.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "8eceba9c4295a162bf268a9eac38a6ad" "CompressedVectorFormats.cs" >}}

## See Also
- Converting SVG to raster formats (PNG, JPEG) with Aspose.Imaging  
- Working with vector rasterization options in Aspose.Imaging  
- Saving images in different vector formats (PDF, EPS) using Aspose.Imaging
