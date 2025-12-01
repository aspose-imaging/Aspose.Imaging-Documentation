---
title: Draw Ellipse Using Aspose.Imaging for .NET
linktitle: Drawing Ellipse
type: docs
weight: 30
url: /net/drawing-ellipse/
description: Demonstrates how to draw ellipses on a bitmap using Aspose.Imaging for .NET.
keywords: ellipse drawing c#
---

# Draw an Ellipse on a Bitmap

## Introduction
This example shows how to create a bitmap image and draw both dotted and solid ellipses on it using the Aspose.Imaging for .NET library. It is useful when you need to add basic vector graphics such as ellipses to raster images.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Access to a writable folder for the output bitmap file

## Step-by-step Guide
1. **Set up the output stream** – Create a `FileStream` pointing to the destination BMP file.
2. **Configure BMP options** – Specify a 32‑bit pixel format and associate the stream with `BmpOptions`.
3. **Create the image** – Use `Image.Create` with the configured options and desired dimensions (e.g., 100 × 100 pixels).
4. **Initialize graphics** – Instantiate a `Graphics` object from the image and clear the canvas with a background colour.
5. **Draw ellipses** –  
   - Use a `Pen` with `Color.Red` to draw a dotted ellipse inside a rectangle.  
   - Use a `Pen` backed by a solid blue brush to draw a continuous ellipse inside another rectangle.
6. **Save and close** – Call `image.Save()` to write the bitmap to the stream and then close all resources.

## Code Example
The following snippet contains the complete implementation of the steps described above.

{{< gist "aspose-imaging-gists" "e92e1bd1576b7afef5549fed29ae6229" "DrawingEllipse.cs" >}}

## See Also
- **Drawing Shapes** – Learn how to draw other geometric shapes such as lines and rectangles.  
- **Working with Brushes** – Explore different brush types for filling shapes.  
- **Saving Images in Different Formats** – Convert and save images to PNG, JPEG, and other formats.
