---
title: Extract a Frame from a WebP Image
linktitle: Extract Frame from WebP
type: docs
weight: 30
url: /net/extract-frame-from-webp-image/
description: Demonstrates how to extract a single frame from a multi‑frame WebP image and save it as BMP.
keywords: webp frame extraction c#
---

# Extract a Frame from a WebP Image

## Introduction
This example shows how to load a multi‑frame WebP image, retrieve a specific frame, and save that frame as a BMP file. Use it when you need to work with individual frames of an animated WebP image.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A WebP image file containing multiple frames (e.g., `asposelogo.webp`)

## Step-by-step Guide
1. **Set up the data folder** – Define the path where the source WebP image and output files reside.  
2. **Load the WebP image** – Create a `WebPImage` instance by loading the source file.  
3. **Check frame count** – Verify that the image contains more than the desired frame index.  
4. **Access the target frame** – Cast the selected page to a `RasterImage`.  
5. **Save the extracted frame** – Use `BmpOptions` to save the raster image as a BMP file.  
6. **Dispose resources** – The `using` statement automatically releases the image resources.

## Code Example
The following code snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "91b7d0bd82b9dd82df758039a018c9e3" "ExtractFrameFromWebPImage.cs" >}}

## See Also
- Converting WebP images to PNG format  
- Resizing WebP images with Aspose.Imaging  
- Extracting frames from animated GIF files
