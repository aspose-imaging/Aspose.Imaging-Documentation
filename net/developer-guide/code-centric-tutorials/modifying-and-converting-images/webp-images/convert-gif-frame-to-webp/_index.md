---
title: Convert GIF Frames to WebP Image
linktitle: Convert GIF Frame to WebP
type: docs
weight: 10
url: /net/convert-gif-frame-to-webp/
description: Demonstrates how to convert each frame of a GIF image into an animated WebP using Aspose.Imaging for .NET.
keywords: gif webp conversion c#
---

# Convert GIF Frames to WebP Image

## Introduction
This example shows how to load a GIF image, extract each frame, and assemble them into an animated WebP image. Use it when you need to migrate animated GIF assets to the more efficient WebP format while preserving animation timing and positioning.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A source GIF file (e.g., **asposelogo.gif**) placed in the example data folder

## Step-by-step Guide
1. **Load the GIF image** using `Image.Load`.
2. **Cast the loaded image** to `GifImage` to access its frame blocks.
3. **Create a new `WebPImage`** with the same dimensions as the source GIF.
4. **Iterate through each `GifFrameBlock`** in the GIF:
   - Convert the GIF frame into a `WebPFrameBlock`.
   - Preserve frame position (`Top`, `Left`) and delay time.
   - Add the WebP frame to the `WebPImage`.
5. **Configure WebP animation options** such as background color, loop count, quality, and lossless mode.
6. **Save the resulting WebP file** to disk.

## Code Example
The following code shows the complete example:

{{< gist "aspose-imaging-gists" "a0c81b764fc7738449d50e230127ad9d" "ConvertGIFFImageFrame.cs" >}}

## See Also
- **Convert WebP to PNG** – how to decode a WebP image into a raster format.  
- **Working with Animated GIFs** – techniques for reading and processing GIF animations.  
- **Optimizing WebP Images** – tips for reducing file size while maintaining quality.
