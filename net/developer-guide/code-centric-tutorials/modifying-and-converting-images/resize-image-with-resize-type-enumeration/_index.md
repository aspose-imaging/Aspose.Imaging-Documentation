---
title: Resize Image Using ResizeType Enumeration
linktitle: Resize Image (ResizeType)
type: docs
weight: 30
url: /net/resize-image-with-resize-type-enumeration/
description: Demonstrates how to resize an image using the ResizeType enumeration in Aspose.Imaging for .NET.
keywords: resize image c#
---

# Resize Image Using ResizeType Enumeration

## Introduction
This example shows how to resize an image by specifying a `ResizeType` enumeration value, allowing you to control the resampling algorithm. Use it when you need precise control over image quality during scaling operations.

## Prerequisites
- .NET 6.0 or later (or any supported .NET version)
- Aspose.Imaging for .NET library
- An input image file (e.g., `aspose-logo.jpg`) placed in the example data directory

## Step-by-step Guide
1. **Prepare the environment** – Ensure the Aspose.Imaging library is referenced via NuGet or a manual assembly reference.  
2. **Load the source image** – Use `Image.Load` to read the image from the data directory.  
3. **Cache the image data** (if not already cached) by calling `image.CacheData()`.  
4. **Resize the width** – Call `image.ResizeWidthProportionally(newWidth, ResizeType.LanczosResample)` to shrink the width using the Lanczos resampling algorithm.  
5. **Resize the height** – Call `image.ResizeHeightProportionally(newHeight, ResizeType.NearestNeighbourResample)` to shrink the height using the nearest‑neighbour algorithm.  
6. **Save the result** – Write the processed image to a new file, e.g., `ResizeImageWithResizeTypeEnumeration_out.png`.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b78bf56465ee23fa1b4c28057d937da7" "ResizeImageWithResizeTypeEnumeration.cs" >}}

## See Also
- **Resize Image Proportionally** – Learn how to resize images while maintaining aspect ratio.  
- **Convert Image Format** – Convert images between different formats using Aspose.Imaging.  
- **Apply Image Filters** – Apply various image-processing filters such as sharpening or blurring.
