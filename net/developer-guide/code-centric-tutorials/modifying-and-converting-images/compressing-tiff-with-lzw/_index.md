---
title: Compress TIFF Images Using LZW Compression
linktitle: Compress TIFF with LZW
type: docs
weight: 30
url: /net/compressing-tiff-with-lzw/
description: Demonstrates how to compress a TIFF image using the LZW algorithm with Aspose.Imaging for .NET.
keywords: tiff compression lzw
---

# Compress TIFF Images Using LZW Compression

## Introduction
This example shows how to reduce the file size of a TIFF image by applying the LZW (Lempel‑Ziv‑Welch) compression algorithm. It is useful when you need loss‑less compression for archival or transmission of high‑quality images.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample TIFF file (e.g., `SampleTiff.tiff`) placed in the example data folder

## Step-by-step Guide
1. **Load the source TIFF image** using `Image.Load`.
2. **Create a `TiffOptions` object** to specify the output format and compression settings.
3. **Configure the options**:
   - Set `BitsPerSample` (e.g., 4‑bit grayscale).
   - Choose `Compression = TiffCompressions.Lzw`.
   - Define `Photometric` mode and assign a suitable grayscale palette.
4. **Save the image** with the configured options, producing a new LZW‑compressed TIFF file.
5. **Verify the output** by checking the file size or opening the resulting image.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "15c92804534b69467126ab5d829487d9" "CompressingTIFFImagesWithLZWAlgorithm.cs" >}}

## See Also
- Converting TIFF to PNG with Aspose.Imaging
- Changing TIFF compression to Deflate
- Working with color palettes in TIFF images
