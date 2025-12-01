---
title: Export an Image to DXF Format
linktitle: Export to DXF
type: docs
weight: 30
url: /net/export-to-dxf/
description: Demonstrates how to convert an EPS image to DXF using Aspose.Imaging for .NET.
keywords: dxf export c#
---

# Export an Image to DXF Format

## Introduction
This example shows how to load an EPS image and save it as a DXF file using Aspose.Imaging for .NET. It is useful when you need to convert vector graphics into a CAD-friendly format while preserving text as lines and handling bezier curves.

## Prerequisites
- .NET 6.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- An EPS source file (e.g., `Pooh group.eps`) placed in the data directory

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder that contains the source EPS file.  
2. **Load the image** – Use `Image.Load` to read the EPS file into an `Image` object.  
3. **Configure DXF options** – Create a `DxfOptions` instance and set:
   * `TextAsLines = true` to convert text to line objects.  
   * `ConvertTextBeziers = true` to approximate text bezier curves.  
   * `BezierPointCount = 20` to define the smoothness of the converted curves.  
4. **Save as DXF** – Call `image.Save` with the target file path and the configured `DxfOptions`.  
5. **Clean up** – Delete the generated DXF file if you only needed it for demonstration purposes.  

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "025334f905cf5b16998540ddf28bf140" "ExportToDxf.cs" >}}

## See Also
- Converting EPS to PDF format
- Exporting raster images to SVG
- Working with DXF options for advanced CAD output
