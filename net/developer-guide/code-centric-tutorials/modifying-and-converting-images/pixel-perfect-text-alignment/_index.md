---
title: Pixel-Perfect Text Alignment Example
linktitle: Pixel-Perfect Text Alignment
type: docs
weight: 30
url: /net/pixel-perfect-text-alignment/
description: Demonstrates how to draw text with precise alignment using Aspose.Imaging for .NET.
keywords: text alignment, c#, aspose imaging
---

# Pixel-Perfect Text Alignment

## Introduction
This example shows how to render text with exact left, center, or right alignment on a PNG image using Aspose.Imaging for .NET. It is useful when you need pixel‑perfect placement of textual annotations or captions in generated graphics.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Access to the sample CDR data folder used by the example (provided with the SDK)

## Step-by-step Guide
1. Determine the base folder that contains the source CDR files.  
2. Define the desired alignments: **Left**, **Center**, and **Right**.  
3. For each alignment, call a helper method that:
   - Creates a new PNG image of the required size.  
   - Initializes a `Graphics` object and clears the canvas to white.  
   - Sets up a `SolidBrush` for drawing text and a `Pen` for drawing guide lines.  
   - Configures a `StringFormat` with `StringFormatFlags.ExactAlignment` and sets its `Alignment` property according to the current alignment.  
   - Iterates through a list of font names and sizes, drawing each string using `Graphics.DrawString`.  
   - Draws horizontal guide lines after each font block and a vertical alignment line at the calculated position.  
   - Saves the image and deletes the temporary file.
4. Run the example to generate three PNG files: `output_Left.png`, `output_Center.png`, and `output_Right.png`.

## Code Example
The full source code for this example is shown below:

{{< gist "aspose-imaging-gists" "bb000c96c26be874a294e8a17ab08352" "PixelPerfectTextAlignment.cs" >}}

## See Also
- [Working with Text Rendering in Aspose.Imaging](#)
- [Creating PNG Images Using Graphics](#)
- [Using StringFormat for Precise Alignment](#)
