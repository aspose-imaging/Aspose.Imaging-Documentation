---
title: Compress TIFF Images Using Adobe Deflate Compression
linktitle: Compress TIFF (Adobe Deflate)
type: docs
weight: 30
url: /net/compressing-tiff-with-adobe-deflate-compression/
description: Demonstrates how to compress TIFF images using Adobe Deflate compression with Aspose.Imaging for .NET.
keywords: tiff compression c#
---

# Compress TIFF Images Using Adobe Deflate Compression

## Introduction
This example shows how to load a TIFF image and save it with Adobe Deflate compression, a lossless compression method suitable for reducing file size while preserving image quality. Use it when you need efficient storage of TIFF files without sacrificing visual fidelity.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample TIFF image (e.g., `SampleTiff1.tiff`) placed in the project’s data directory

## Step-by-step Guide
1. **Initialize the environment** – Ensure Aspose.Imaging is referenced in the project and a valid license is applied if required.  
2. **Load the source TIFF image** – Use `Image.Load` to read the original TIFF file from disk.  
3. **Configure TIFF output options** – Create a `TiffOptions` instance, set `BitsPerSample`, `Photometric`, and assign `Compression = TiffCompressions.AdobeDeflate`.  
4. **Define a grayscale palette (optional)** – For 4‑bit images, create a grayscale palette via `ColorPaletteHelper.Create4BitGrayscale`.  
5. **Save the image** – Persist the modified image using the configured `TiffOptions` to apply Adobe Deflate compression.  

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "280f554fed35a9ac4c51253b677416f9" "CompressingTIFFImagesWithAdobeDeflateCompression.cs" >}}

## See Also
- Converting TIFF images to other formats with Aspose.Imaging  
- Changing TIFF compression types (LZW, CCITT, etc.)  
- Working with color palettes in TIFF images
