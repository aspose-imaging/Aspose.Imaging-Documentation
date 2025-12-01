---
title: Save a Raster Image to TIFF with Compression
linktitle: Save Raster Image to TIFF
type: docs
weight: 30
url: /net/saving-raster-image-to-tiff-with-compression/
description: Demonstrates how to save a raster image as a TIFF file using a specific compression method.
keywords: tiff compression c#
---

# Save a Raster Image to TIFF with Compression

## Introduction
This example shows how to load a raster image, apply TIFF-specific options, and save it as a compressed TIFF file. Use it when you need to reduce file size while preserving image quality in TIFF format.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0 in the source tree)
- Aspose.Imaging for .NET library
- A sample TIFF image (e.g., `SampleTiff1.tiff`) placed in the working directory

## Step-by-step Guide
1. **Create `TiffOptions`** – instantiate `TiffOptions` and configure bits per sample, photometric interpretation, resolution, and planar configuration.  
2. **Set Compression** – assign the desired compression algorithm (e.g., `AdobeDeflate` or `Deflate`).  
3. **Load the source raster image** – use `Image.Load` to read the existing TIFF file into a `RasterImage`.  
4. **Create a `TiffImage`** – wrap the raster image in a `TiffFrame` and pass it to the `TiffImage` constructor.  
5. **Save the output** – call `Save` on the `TiffImage` instance, providing the output path and the configured `TiffOptions`.

## Code Example
The complete source code for this workflow is shown below.

{{< gist "aspose-imaging-gists" "103b21d30e8853c2efbe6f8eae5f3ac8" "SavingRasterImageToTIFFWithCompression.cs" >}}

## See Also
- Saving a raster image to JPEG with quality settings  
- Converting images to PNG format with custom options  
- Working with multi-page TIFF files in Aspose.Imaging
