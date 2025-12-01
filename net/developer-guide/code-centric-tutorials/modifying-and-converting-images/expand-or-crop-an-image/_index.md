---
title: Expand or Crop an Image
linktitle: Expand or Crop
type: docs
weight: 30
url: /net/expand-or-crop-an-image/
description: Demonstrates how to expand or crop an image by defining a custom rectangle.
keywords: crop image c#
---

# Expand or Crop an Image

## Introduction
This example illustrates how to expand or crop an image using Aspose.Imaging for .NET by specifying a custom rectangle. It is useful when you need to adjust the visible area of an image, either by enlarging the canvas or extracting a specific region.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An input JPEG image (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Load the source image into a `RasterImage` instance and cache its data.
2. Create a `Rectangle` object that defines the X, Y coordinates, width, and height of the desired region. Negative X/Y values expand the canvas, while positive values within the original bounds crop the image.
3. Save the resulting image using `RasterImage.Save`, passing the rectangle to indicate the target area.
4. Verify the output file (e.g., `Grayscaling_out.jpg`) contains the expanded or cropped region.

## Code Example
Below is the complete C# code for this scenario:

{{< gist "aspose-imaging-gists" "c31e7d45ae337183698a4082d5565680" "ExpandOrCropAnImage.cs" >}}

## See Also
- **Resizing Images** – Learn how to resize images while maintaining aspect ratio.  
- **Rotating Images** – Apply rotation transformations to images using Aspose.Imaging.  
- **Applying Image Filters** – Explore how to apply various filters, such as grayscale or blur, to images.
