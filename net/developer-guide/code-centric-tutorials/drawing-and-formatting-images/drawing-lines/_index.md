---
title: Draw Lines on an Image using Aspose.Imaging for .NET
linktitle: Drawing Lines
type: docs
weight: 30
url: /net/drawing-lines/
description: Creates a bitmap, fills it with a background color, and draws solid and dotted lines.
keywords: draw lines c# aspose-imaging
---

# Draw Lines on an Image using Aspose.Imaging for .NET

## Introduction
This example demonstrates how to create a new bitmap image, set a background color, and draw both solid and dotted lines using Aspose.Imaging for .NET. Use it when you need to programmatically add line graphics to images.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- No additional external files are required; the example generates the output image in code.

## Step-by-step Guide
1. **Create a bitmap stream** – Initialize a `FileStream` pointing to the output file path.
2. **Configure bitmap options** – Set `BitsPerPixel` and assign the stream as the source.
3. **Instantiate an image** – Use `Image.Create` with the bitmap options and define the image size.
4. **Initialize graphics** – Create a `Graphics` object from the image and clear it with a background color.
5. **Draw lines** –  
   - Use a `Pen` with a solid blue color to draw two diagonal dotted lines.  
   - Use `Pen` objects with `SolidBrush` of various colors to draw four continuous lines forming a rectangle.
6. **Save the image** – Call `image.Save()` to write the output to the stream.

## Code Example
The following code demonstrates how to draw lines:

{{< gist "aspose-imaging-gists" "1b8494e881eb50cd6b06165d67f8b572" "DrawingLines.cs" >}}

## See Also
- **Drawing Shapes** – Learn how to draw rectangles, ellipses, and other shapes.  
- **Working with Colors and Brushes** – Explore different brushes and color options for graphics.  
- **Saving Images in Different Formats** – Convert and save images to JPEG, PNG, and other formats.
