---
title: Draw Vector Image to Raster Image
linktitle: Draw Vector Image
type: docs
weight: 30
url: /net/draw-vector-image-to-raster-image/
description: Rasterize an SVG to PNG, draw it onto the original vector image, and save the combined result.
keywords: draw vector image c#
---

# Draw Vector Image to Raster Image

## Introduction
This example demonstrates how to rasterize an SVG file to a PNG image, render the raster image onto the original SVG using Aspose.Imaging's graphics API, and finally save the combined drawing as a new SVG file. Use it when you need to blend raster content with vector graphics while preserving scalability.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input SVG file (`asposenet_220_src02.svg`) placed in the example data directory

## Step-by-step Guide
1. **Set up the data directory** – Obtain the folder that contains the source SVG.
2. **Load the SVG image** – Use `Image.Load` to read the SVG as an `SvgImage`.
3. **Configure rasterization options** – Create a `SvgRasterizationOptions` instance and set its `PageSize` to match the SVG size.
4. **Rasterize to PNG** – Create `PngOptions`, assign the rasterization options, and save the SVG to a `MemoryStream` as PNG.
5. **Load the raster image** – Reset the stream position and load the PNG into a `RasterImage`.
6. **Create an `SvgGraphics2D` object** – This enables drawing operations on the original SVG.
7. **Calculate scaled dimensions** – Reduce the raster image size by half and compute the centered origin point.
8. **Draw the raster image onto the SVG** – Call `graphics.DrawImage` with the calculated bounds.
9. **Finalize and save** – End the recording to obtain the resulting `SvgImage` and save it to a new file.

## Code Example
The complete code is shown below:

{{< gist "aspose-imaging-gists" "7c125ae34666c88af70bfa6f39c9a4fe" "DrawVectorImageToRasterImage.cs" >}}

## See Also
- **Converting SVG to Raster Formats** – Learn how to convert vector graphics to PNG, JPEG, and other raster formats.
- **Drawing Shapes on Raster Images** – Explore drawing primitives such as lines, rectangles, and circles on raster images using Aspose.Imaging.
