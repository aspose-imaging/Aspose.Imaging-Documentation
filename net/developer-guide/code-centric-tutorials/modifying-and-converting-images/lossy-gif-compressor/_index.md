---
title: Compress GIF Images Using Lossy Compression
linktitle: Lossy GIF Compression
type: docs
weight: 30
url: /net/lossy-gif-compressor/
description: Demonstrates how to apply lossy compression to GIF images with Aspose.Imaging for .NET.
keywords: gif compression c#
---

# Compress GIF Images Using Lossy Compression

## Introduction
This example shows how to reduce the size of animated GIF files by applying lossy compression. Use it when you need smaller GIFs without a noticeable loss in visual quality.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An input GIF file named `anim_orig.gif` placed in the working directory

## Step-by-step Guide
1. **Set up the environment** – Ensure the Aspose.Imaging NuGet package is referenced in your project.  
2. **Define compression options** – Create a `GifOptions` instance and set the `MaxDiff` property to control the level of lossy compression (e.g., 80 for balanced compression).  
3. **Load the source image** – Use `Image.Load` to read the original GIF file.  
4. **Save with lossy settings** – Call `Image.Save` with the configured `GifOptions` to produce a compressed GIF file (e.g., `anim_lossy-80.gif`).  

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "bb0a98b09e0506d3453bcf9a2b82fe91" "ImplementationOfLossyGIFCompressor.cs" >}}

## See Also
- [Saving Images in Different Formats](../saving-images-different-formats)
- [Optimizing Image Quality with Aspose.Imaging](../optimizing-image-quality)
- [Working with Animated GIFs](../animated-gif-handling)
