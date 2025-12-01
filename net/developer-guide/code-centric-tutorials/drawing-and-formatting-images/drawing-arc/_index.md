---
title: Draw an Arc on an Image using Aspose.Imaging for .NET
linktitle: Drawing Arc
type: docs
weight: 30
url: /net/drawing-arc/
description: Creates a BMP image, clears the background, and draws an arc shape using Aspose.Imaging for .NET.
keywords: draw arc c#
---

# Draw an Arc on an Image

## Introduction
This example demonstrates how to create a bitmap image, set a background color, and draw an arc shape with a specified pen. Use it when you need to add curved markings or decorative elements to images programmatically.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library
- No external files are required; the example generates its own output image.

## Step-by-step Guide
1. **Create BMP options** – configure `BitsPerPixel` and assign a `StreamSource` for the output file.  
2. **Instantiate the image** – use `Image.Create` with the defined options and desired dimensions (e.g., 100 × 100 pixels).  
3. **Initialize graphics** – create a `Graphics` object from the image and clear the canvas with a background color (e.g., Yellow).  
4. **Configure the pen** – set the pen color (e.g., Black) that will be used to draw the arc.  
5. **Draw the arc** – call `Graphics.DrawArc`, specifying the pen, bounding rectangle coordinates, width, height, start angle, and sweep angle.  
6. **Save the image** – invoke `image.Save()` to write the output BMP file to the stream.

## Code Example
The following snippet shows the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "09cc219a6372f5ff214072c9c1584e98" "DrawingArc.cs" >}}

## See Also
- **Drawing Lines and Shapes** – learn how to draw other geometric primitives such as lines, rectangles, and ellipses.  
- **Saving Images in Different Formats** – explore how to save images in PNG, JPEG, and other supported formats.  
- **Working with Graphics Transformations** – apply scaling, rotation, and translation to graphics objects for advanced rendering.
