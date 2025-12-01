---
title: Resize an Image Using the ResizeType Enumeration
linktitle: Resizing with ResizeType
type: docs
weight: 30
url: /net/resizing-with-resize-type-enumeration/
description: Resize an image using the LanczosResample ResizeType enumeration.
keywords: resize image c#
---

# Resize an Image Using the ResizeType Enumeration

## Introduction
This example demonstrates how to resize an image while specifying a `ResizeType` enumeration value. Use it when you need high‑quality resampling, such as when preparing thumbnails or adjusting image dimensions for different devices.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Input image file (e.g., `aspose-logo.jpg`) placed in the sample data folder

## Step-by-step Guide
1. **Set up the data directory** – locate the folder that contains the source image.  
2. **Load the image** – use `Image.Load` to read the source file into an `Image` object.  
3. **Resize the image** – call `image.Resize(width, height, ResizeType.LanczosResample)` to resize with the Lanczos resampling algorithm.  
4. **Save the result** – write the resized image to a new file, such as `SimpleResizing_out.jpg`.  

## Code Example
The following code snippet shows the complete example:

{{< gist "aspose-imaging-gists" "ef79a309336c6c6da260722fa52a9531" "ResizingWithResizeTypeEnumeration.cs" >}}

## See Also
- **Image Resizing Options** – explore other `ResizeType` values and when to use them.  
- **Saving Images in Different Formats** – learn how to export the resized image to PNG, BMP, or TIFF.  
- **Batch Image Processing** – process multiple images in a loop using Aspose.Imaging.
