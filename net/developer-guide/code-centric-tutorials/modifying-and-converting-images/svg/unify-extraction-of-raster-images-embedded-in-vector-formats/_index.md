---
title: Extract Raster Images from SVG and Clean Up
linktitle: Extract Raster Images from SVG
type: docs
weight: 30
url: /net/unify-extraction-of-raster-images-embedded-in-vector-formats/
description: Demonstrates how to extract embedded raster images from an SVG file and delete them after processing using Aspose.Imaging for .NET.
keywords: svg raster extraction
---

# Extract Raster Images from SVG

## Introduction
This example shows how to load an SVG file, retrieve all embedded raster images, save each image to a separate file, and finally clean up by deleting the extracted files. Use it when you need to work with raster assets embedded inside vector graphics.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- An SVG file containing embedded raster images (e.g., `test2.svg`)

## Step-by-step Guide
1. **Load the SVG file** using `Image.Load`.
2. **Retrieve embedded images** via `VectorImage.GetEmbeddedImages()`.
3. **Iterate through each `EmbeddedImage`**, determine its file format, and save it to a temporary file.
4. **Collect the paths** of the saved images.
5. **Delete the temporary files** after they are no longer needed.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "a673c350b7a320c3d315a430b475c0f0" "UnifyExtractionOfRasterImagesEmbeddedInVectorFormats.cs" >}}

## See Also
- Converting SVG to raster formats
- Modifying vector images with Aspose.Imaging
- Working with embedded images in PDF files
