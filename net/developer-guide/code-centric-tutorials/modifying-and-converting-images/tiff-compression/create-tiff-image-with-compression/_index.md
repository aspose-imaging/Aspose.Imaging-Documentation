---
title: Create a TIFF Image with Compression using Aspose.Imaging for .NET
linktitle: Create TIFF with Compression
type: docs
weight: 30
url: /net/create-tiff-image-with-compression/
description: Demonstrates how to create a TIFF image and apply compression options with Aspose.Imaging for .NET.
keywords: tiff compression asp.net
---

# Create a TIFF Image with Compression

## Introduction
This example shows how to generate a new TIFF image, configure its compression settings, and save the result. Use it when you need to create TIFF files with specific compression types such as AdobeDeflate or Deflate.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Access to a writable folder for the output TIFF file

## Step-by-step Guide
1. **Create `TiffOptions`** – Set image dimensions, photometric format, resolution, and planar configuration.  
2. **Select Compression** – Choose a compression algorithm (`AdobeDeflate` or `Deflate`) via the `Compression` property.  
3. **Instantiate `TiffImage`** – Use the configured options to create a new `TiffImage` with a frame of the desired size.  
4. **Manipulate Pixels (optional)** – Set pixel colors as needed (e.g., drawing a red diagonal).  
5. **Save the Image** – Call `Save` on the `TiffImage` instance, providing the target file path.

## Code Example
Below is the complete code for this workflow.

{{< gist "aspose-imaging-gists" "27602dca80923d6237fee645e1446764" "CreatingTIFFImageWithCompression.cs" >}}

## See Also
- **Saving Raster Images to Different Formats** – Learn how to save images in formats other than TIFF.  
- **Applying Different Compression Types** – Explore other compression options available for TIFF images.  
- **Modifying Existing TIFF Files** – See how to open and edit an existing TIFF image.
