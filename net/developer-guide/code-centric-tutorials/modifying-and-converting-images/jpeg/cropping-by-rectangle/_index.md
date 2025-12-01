---
title: Crop JPEG Image by Rectangle with Aspose.Imaging for .NET
linktitle: Crop JPEG by Rectangle
type: docs
weight: 30
url: /net/cropping-by-rectangle/
description: Demonstrates how to crop a JPEG image using a rectangle region.
keywords: crop jpeg c#
---

# Crop JPEG Image by Rectangle

## Introduction
This example illustrates how to crop a JPEG image by specifying a rectangular area. Use it when you need to extract a specific part of a JPEG file without altering the rest of the image.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- A source JPEG image (e.g., `aspose-logo.jpg`) placed in the data directory

## Step-by-step Guide
1. Obtain the path to the folder that contains the source JPEG image.  
2. Load the JPEG file into a `RasterImage` instance using `Image.Load`.  
3. Ensure the image data is cached by calling `CacheData` if necessary.  
4. Define a `Rectangle` with the desired X, Y coordinates and width, height.  
5. Call the `Crop` method on the `RasterImage` instance, passing the rectangle.  
6. Save the cropped image to a new JPEG file.

## Code Example
The following example shows how to crop a JPEG image using a rectangle:

{{< gist "aspose-imaging-gists" "2c872364943e3b2f2256414328a6da93" "CroppingByRectangle.cs" >}}

## See Also
- Converting JPEG to PNG with Aspose.Imaging for .NET  
- Resizing images using Aspose.Imaging for .NET  
- Rotating an image with Aspose.Imaging for .NET
