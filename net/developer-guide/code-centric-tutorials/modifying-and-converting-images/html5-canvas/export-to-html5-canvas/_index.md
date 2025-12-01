---
title: Export SVG to HTML5 Canvas
linktitle: Export to HTML5 Canvas
type: docs
weight: 30
url: /net/export-to-html5-canvas/
description: Demonstrates how to convert an SVG image into an HTML5 canvas file using Aspose.Imaging for .NET.
keywords: html5 canvas, svg, aspose imaging
---

# Export SVG to HTML5 Canvas

## Introduction
This example shows how to load an SVG file and save it as an HTML5 canvas document. Use it when you need to render vector graphics in web browsers that support the `<canvas>` element.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample SVG file (e.g., `Sample.svg`) placed in the data directory

## Step-by-step Guide
1. Obtain the path to the data directory that contains the SVG file.  
2. Load the SVG image using `Image.Load`.  
3. Create an `Html5CanvasOptions` instance and configure rasterization settings (e.g., page width and height).  
4. Call `image.Save` with the output HTML file name and the configured options.  
5. Verify that the generated HTML file contains a `<canvas>` element rendering the SVG content.

## Code Example
Below is the complete code snippet for this task:

{{< gist "aspose-imaging-gists" "b2017daa35288c46be70d41a3568c240" "ExportToHtml5Canvas.cs" >}}

## See Also
- Converting SVG to raster formats (PNG, JPEG) with Aspose.Imaging
- Exporting images to PDF using Aspose.Imaging
- Working with vector rasterization options in Aspose.Imaging
