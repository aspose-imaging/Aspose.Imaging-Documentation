---
title: Convert GIF Image Layers to TIFF
linktitle: Convert GIF Layers to TIFF
type: docs
weight: 30
url: /net/convert-gif-image-layers-to-tiff/
description: Demonstrates how to extract each frame from a GIF image and save it as separate TIFF files using Aspose.Imaging for .NET.
keywords: gif tiff conversion
---

# Convert GIF Image Layers to TIFF

## Introduction
This example shows how to iterate through the frames (layers) of a GIF image and save each frame as an individual TIFF file. Use it when you need to work with GIF frames separately or convert animated GIFs into a series of static TIFF images.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A GIF file (e.g., `asposelogo.gif`) placed in the example data directory

## Step-by-step Guide
1. **Load the GIF image** using `Image.Load`.
2. **Cast the loaded image to `GifImage`** to access GIF‑specific members.
3. **Iterate through the `Blocks` collection** of the GIF image.
4. **Identify `GifFrameBlock` objects** – these represent individual frames.
5. **Create a `TiffOptions` instance** to specify TIFF saving parameters.
6. **Save each frame** with `GifFrameBlock.Save`, providing a unique file name and the TIFF options.

## Code Example
Below is the complete code snippet for this process.

{{< gist "aspose-imaging-gists" "24ff0cf2c8ceff324a47a179d4e303c7" "ConvertGIFImageLayersToTIFF.cs" >}}

## See Also
- [Convert Multi‑Page TIFF to Separate Images](#)
- [Create a New GIF Image from Multiple Frames](#)
