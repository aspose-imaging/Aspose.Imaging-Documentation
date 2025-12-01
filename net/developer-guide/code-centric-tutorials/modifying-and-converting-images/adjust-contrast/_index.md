---
title: Adjust Image Contrast with Aspose.Imaging for .NET
linktitle: Adjust Contrast
type: docs
weight: 30
url: /net/adjust-contrast/
description: Demonstrates how to adjust the contrast of an image and save it as TIFF using Aspose.Imaging for .NET.
keywords: adjust contrast c#
---

# Adjust Image Contrast

## Introduction
This example shows how to modify the contrast of a raster image and then save the result as a TIFF file. Use it when you need to enhance visual quality or prepare images for further processing.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input image file (e.g., `aspose-logo.jpg`) placed in the sample data folder

## Step-by-step Guide
1. **Initialize the data directory** – obtain the path to the folder that contains the source image.  
2. **Load the image** – use `Image.Load` to read the source file into an `Image` object.  
3. **Cast to `RasterImage`** – most pixel‑level operations, including contrast adjustment, require a `RasterImage`.  
4. **Cache image data (optional)** – call `CacheData` if the raster image is not already cached for better performance.  
5. **Adjust the contrast** – invoke `AdjustContrast(int)` with the desired contrast value (e.g., `10`).  
6. **Configure TIFF output options** – create a `TiffOptions` instance and set properties such as `BitsPerSample` and `Photometric`.  
7. **Save the processed image** – call `Save` on the raster image, passing the output file name and the TIFF options.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "7aed6b8dc7237134650a3e30020e96ea" "AdjustContrast.cs" >}}

## See Also
- [Resize an Image](../resize-image/)
- [Convert Image Format](../convert-image-format/)
- [Apply Image Filters](../apply-image-filters/)
