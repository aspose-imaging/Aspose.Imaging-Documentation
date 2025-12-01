---
title: Compress BMP Image Using RLE4 Compression with Aspose.Imaging for .NET
linktitle: BMP RLE4 Compression
type: docs
weight: 30
url: /net/bmp-rle4/
description: Demonstrates how to load a BMP image and save it with RLE4 compression using Aspose.Imaging for .NET.
keywords: bmp compression c#
---


# Compress BMP Image Using RLE4 Compression

## Introduction
This example shows how to load a BMP image, apply RLE4 (Run‑Length Encoding 4‑bit) compression, and save the result. Use it when you need to reduce the file size of 4‑bit BMP images while preserving palette information.

## Prerequisites
- .NET 9.0 (or later)  
- Aspose.Imaging for .NET library  
- A sample BMP file named **Rle4.bmp** placed in the data directory used by the examples  

## Step-by-step Guide
1. Obtain the path to the folder containing the source BMP file.  
2. Load the BMP image using `Image.Load`.  
3. Create a `BmpOptions` instance and set:  
   - `Compression = BitmapCompression.Rle4`  
   - `BitsPerPixel = 4`  
   - `Palette = ColorPaletteHelper.Create4Bit()` to provide a 4‑bit palette.  
4. Save the image with the configured options to a new file (e.g., **output.bmp**).  
5. Optionally delete the generated output file after verification.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "dd8158f55b5eb6f06bc830d825691b6d" "BmpRLE4.cs" >}}

## See Also
- [Saving BMP Images with Different Bit Depths](#)  
- [Using Color Palettes with Aspose.Imaging](#)  
- [Compressing Images with Other BMP Compression Types](#)
