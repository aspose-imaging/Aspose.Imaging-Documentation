---
title: Support Full-Frame GIF Conversion to TIFF
linktitle: Full-Frame GIF to TIFF
type: docs
weight: 30
url: /net/support-of-full-frame-gif/
description: Demonstrates how to save a GIF image as a full‑frame or non‑full‑frame multi‑page TIFF using Aspose.Imaging for .NET.
keywords: gif tiff full-frame
---

# Support Full-Frame GIF Conversion to TIFF

## Introduction
This example shows how to convert an animated GIF into a multi‑page TIFF file while optionally preserving each frame as a full‑frame image. Use it when you need TIFF output for GIF animations with or without full‑frame frames.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- An input GIF file (e.g., **Animation.gif**) placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the example data directory that contains **Animation.gif**.  
2. Load the GIF image using `Image.Load`.  
3. Save the image as a TIFF file with `FullFrame = true` to create a full‑frame multi‑page TIFF.  
4. Save the same image as a TIFF file without setting `FullFrame` to create a non‑full‑frame version.  
5. (Optional) Delete the generated TIFF files after processing.

## Code Example
The following code demonstrates the full process:

{{< gist "aspose-imaging-gists" "1dfd00f0bdb5f61fd8a714c375e14723" "SupportOfFullFrameGif.cs" >}}

## See Also
- Converting GIF images to other formats with Aspose.Imaging
- Working with multi‑page TIFF images in Aspose.Imaging
- Modifying image frames and properties using Aspose.Imaging for .NET
