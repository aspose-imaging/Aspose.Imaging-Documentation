---
title: Add Frames to a TIFF Image
linktitle: Add Frames to TIFF
type: docs
weight: 30
url: /net/add-frames-to-tiff-image/
description: Demonstrates how to combine multiple JPEG images into a multi‑frame TIFF file using Aspose.Imaging for .NET.
keywords: tiff frames c#
---

# Add Frames to a TIFF Image

## Introduction
This example shows how to create a new TIFF image and add multiple JPEG frames to it, resulting in a multi‑page TIFF document. Use it when you need to bundle several raster images into a single TIFF file for archival, printing, or distribution.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A folder containing JPEG (`*.jpg`) files that will be added as frames

## Step-by-step Guide
1. **Create a TIFF image** with the desired width, height, and compression options using `TiffOptions`.
2. **Iterate over the source JPEG files** in the data directory.
3. **Load each JPEG**, resize it to match the TIFF dimensions, and obtain its pixel data.
4. **Create a new `TiffFrame`** for each image (the first image uses the active frame, subsequent images require a new frame instance).
5. **Save the pixel data** from the resized JPEG into the current TIFF frame.
6. **Add the frame** to the TIFF image collection when it is not the first frame.
7. **Save the final multi‑frame TIFF** to disk.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "9a457e803b3ae070644aa1fb1a33214b" "AddFramesToTIFFImage.cs" >}}

## See Also
- **Convert JPEG to TIFF** – Learn how to convert a single JPEG image to a TIFF file.  
- **Resize Images** – Explore resizing techniques with Aspose.Imaging.  
- **Create Multi‑Page PDF** – Add multiple pages to a PDF document using Aspose.PDF.
