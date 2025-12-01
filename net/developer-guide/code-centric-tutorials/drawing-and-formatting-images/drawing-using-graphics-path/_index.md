---
title: Draw Shapes Using GraphicsPath in Aspose.Imaging for .NET
linktitle: Drawing Using GraphicsPath
type: docs
weight: 30
url: /net/drawing-using-graphics-path/
description: Demonstrates how to draw shapes and fill them using GraphicsPath with Aspose.Imaging for .NET.
keywords: graphicspath, draw shapes, c#
---

# Draw Shapes Using GraphicsPath in Aspose.Imaging for .NET

## Introduction
This example shows how to create vector graphics using `GraphicsPath` and render them onto an image with Aspose.Imaging for .NET. Use it when you need to combine geometric shapes, text, and custom brushes in a single drawing operation.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample bitmap file (`sample_1.bmp`) placed in the example data directory

## Step-by-step Guide
1. Create `BmpOptions` and set the desired bits per pixel.  
2. Initialize an `Image` object with the specified dimensions and options.  
3. Obtain a `Graphics` instance from the image and clear the background.  
4. Build a `GraphicsPath`:
   - Create a `Figure`.
   - Add an `EllipseShape`, `RectangleShape`, and `TextShape` to the figure.
   - Add the figure to the `GraphicsPath`.
5. Draw the path on the graphics surface using a `Pen`.  
6. Create a `HatchBrush` with custom foreground and background colors and fill the path.  
7. Save the image to persist the drawing.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "757711e245ecb6316f0aafd850340d16" "DrawingUsingGraphicsPath.cs" >}}

## See Also
- [Creating and Saving Images with Aspose.Imaging](https://docs.aspose.com/imaging/net/creating-and-saving-images/)
- [Using Brushes and Pens for Advanced Drawing](https://docs.aspose.com/imaging/net/using-brushes-and-pens/)
- [Working with Text Rendering in Aspose.Imaging](https://docs.aspose.com/imaging/net/text-rendering/)
