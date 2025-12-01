---
title: Convert Other Image Formats to SVG
linktitle: Convert to SVG
type: docs
weight: 30
url: /net/converting-other-formats-to-svg/
description: Demonstrates how to convert images of various formats to SVG using Aspose.Imaging for .NET.
keywords: svg conversion c#
---

# Convert Other Image Formats to SVG

## Introduction
This example shows how to load an image in any supported format and save it directly as an SVG file using Aspose.Imaging for .NET. Use it when you need vector‑based output for raster or other image types.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library installed
- Input image file(s) placed in the `DataDir_SVG` folder (provided with the examples)

## Step-by-step Guide
1. Obtain the path to the directory that contains the source image (`RunExamples.GetDataDir_SVG()`).
2. Load the source image using `Image.Load`.
3. Open a `FileStream` for the destination SVG file.
4. Call `image.Save(fileStream)` to write the image in SVG format.
5. Dispose of the `Image` and `FileStream` objects (handled by `using` statements).

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "851182ca9d8f231772ba3a153106348b" "ConvOfOtherFormatsToSVG.cs" >}}

## See Also
- Converting raster images to PNG
- Exporting images to PDF format
- Working with SVG images in Aspose.Imaging
