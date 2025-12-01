---
title: Creating a WMF Metafile Image with Aspose.Imaging
linktitle: Create WMF Metafile Image
type: docs
weight: 30
url: /net/create-wmf-meta-file-image/
description: Example demonstrating how to create and draw on a WMF metafile image using Aspose.Imaging for .NET.
keywords: wmf metafile c# drawing
---

# Create a WMF Metafile Image

## Introduction
This example shows how to generate a WMF (Windows Metafile) image, draw various shapes, text, and other images onto it, and then save the result. Use it when you need vector‑based graphics that can be edited by Windows applications.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- No additional files are required; the example creates and saves the WMF file in the output folder.

## Step-by-step Guide
1. **Create a graphics recorder** – Instantiate `WmfRecorderGraphics2D` with a drawing rectangle and DPI.
2. **Set background and drawing tools** – Define background color, `Pen`, and `Brush` objects.
3. **Draw shapes** – Use methods such as `FillPolygon`, `DrawEllipse`, `DrawArc`, `DrawCubicBezier`, etc., to render vector graphics.
4. **Render an existing raster image** – Load an image with `Image.Load`, cast to `RasterImage`, and draw it onto the canvas.
5. **Add text** – Create a `Font` and draw a string with `DrawString`.
6. **Finalize the WMF image** – Call `EndRecording` to obtain a `WmfImage` and save it to disk.

## Code Example
The following snippet runs the complete workflow described above:

{{< gist "aspose-imaging-gists" "83c15fb75937a059fe680a9c13d315e8" "CreateWMFMetaFileImage.cs" >}}

## See Also
- [Converting WMF to other formats](#)  
- [Working with vector graphics in Aspose.Imaging](#)  
- [Saving images to different file types](#)
