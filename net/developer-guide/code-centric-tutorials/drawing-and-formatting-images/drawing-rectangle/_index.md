---
title: Draw Rectangles on an Image using Aspose.Imaging for .NET
linktitle: Draw Rectangles
type: docs
weight: 30
url: /net/drawing-rectangle/
description: Creates a bitmap, draws two colored rectangles, and saves the result.
keywords: drawing rectangle image c#
---

# Draw Rectangles on an Image using Aspose.Imaging for .NET

## Introduction
This example demonstrates how to create a bitmap image, clear its background, and draw two rectangles with different colors using Aspose.Imaging for .NET. Use it when you need to add simple geometric shapes to an image programmatically.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- No external files are required; the example generates the image in memory.

## Step-by-step Guide
1. Define the output path for the bitmap image.
2. Create a `BmpOptions` object and set the desired bits‑per‑pixel and source stream.
3. Instantiate an `Image` with the specified dimensions using the BMP options.
4. Obtain a `Graphics` object from the image.
5. Clear the drawing surface with a background color (e.g., Yellow).
6. Draw the first rectangle using a red pen.
7. Draw the second rectangle using a blue solid brush pen.
8. Save the image to the file system.

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "099c18cf52715b43b653004ba35276a3" "DrawingRectangle.cs" >}}

## See Also
- **Filling Shapes** – Learn how to fill rectangles and other shapes with brushes.  
- **Working with Colors** – Explore color manipulation and custom color creation.  
- **Saving Images in Different Formats** – Convert and save images to PNG, JPEG, and other formats.
