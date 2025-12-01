---
title: Concatenating TIFF Images
linktitle: Concat TIFF Images
type: docs
weight: 30
url: /net/concat-tiff-images/
description: Demonstrates how to merge multiple TIFF frames into a single TIFF image using Aspose.Imaging for .NET.
keywords: tiff concat c#
---

# Concatenate TIFF Images

## Introduction
This example shows how to combine separate TIFF files or frames into a single multi‑frame TIFF image. Use it when you need to create a consolidated TIFF document from individual pages or images.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample TIFF files (`demo.tif`, `sample.tif`) placed in the example data directory

## Step-by-step Guide
1. Copy the source TIFF to a working copy to avoid modifying the original file.  
2. Load the destination TIFF image using `TiffImage`.  
3. Load the source TIFF image that contains the frame you want to add.  
4. Use `TiffFrame.CopyFrame` to duplicate the active frame from the source image.  
5. Add the copied frame to the destination image with `AddFrame`.  
6. Save the resulting multi‑frame TIFF to the output file.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "3b0cd885a92bf60e8b2065200a1a40b6" "ConcatTIFFImages.cs" >}}

## See Also
- [Working with Multi‑Page TIFF Images](#)
- [Adding Watermarks to TIFF Files](#)
- [Converting TIFF to Other Formats](#)
