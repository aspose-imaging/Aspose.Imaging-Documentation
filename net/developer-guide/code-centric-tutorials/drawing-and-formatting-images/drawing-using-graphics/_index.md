---
title: Drawing Using Graphics with Aspose.Imaging for .NET
linktitle: Drawing Using Graphics
type: docs
weight: 30
url: /net/drawing-using-graphics/
description: Demonstrates how to draw shapes and fill polygons using the Graphics class in Aspose.Imaging for .NET.
keywords: drawing graphics c#
---

# Drawing Using Graphics with Aspose.Imaging for .NET

## Introduction
This example shows how to create a bitmap image, obtain a `Graphics` object, and use it to draw basic shapes such as ellipses and polygons. It is useful when you need to programmatically add vector graphics to raster images.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library installed via NuGet or manual reference
- A sample image file (e.g., `SampleImage_out.bmp`) placed in the example data directory

## Step-by-step Guide
1. Create `BmpOptions` and configure the bit depth (24 bits per pixel).  
2. Set the source of the image to a `FileCreateSource` that points to the output BMP file.  
3. Use `Image.Create` to instantiate a blank image with the desired dimensions (500 × 500).  
4. Obtain a `Graphics` instance from the image.  
5. Clear the drawing surface with a background color (white).  
6. Create a `Pen` with the desired stroke color (blue) and draw an ellipse using `Graphics.DrawEllipse`.  
7. Create a `LinearGradientBrush` for a gradient fill, then draw a filled polygon using `Graphics.FillPolygon`.  
8. Save the image to persist the drawn graphics.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b539cea1034f74fac74904197f64576d" "DrawingUsingGraphics.cs" >}}

## See Also
- **Working with Brushes** – Learn how to use different brush types for filling shapes.  
- **Saving Images in Different Formats** – Explore options for exporting images to PNG, JPEG, and other formats.  
- **Manipulating Image Pixels** – Understand how to access and modify individual pixel data.
