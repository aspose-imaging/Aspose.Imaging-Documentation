---
title: Convert CMX Images to PNG with Aspose.Imaging for .NET
linktitle: CMX to PNG Conversion
type: docs
weight: 30
url: /net/cmx-to-png-conversion/
description: Demonstrates how to convert CMX vector images to PNG using Aspose.Imaging for .NET.
keywords: cmx png conversion
---

# Convert CMX Images to PNG

## Introduction
This example shows how to load CMX vector files and rasterize them into high‑quality PNG images. Use it when you need to transform Corel Metafile (CMX) documents into a widely supported raster format for web or printing.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A set of CMX sample files (e.g., `Rectangle.cmx`, `Ellipse.cmx`, etc.)

## Step-by-step Guide
1. Obtain the directory that contains the CMX source files.  
2. Define an array with the names of the CMX files you want to convert.  
3. For each file:
   - Load the CMX image using `Image.Load`.  
   - Save the image as PNG by providing a `PngOptions` object configured with `CmxRasterizationOptions`.  
   - Set rasterization properties such as `Positioning` and `SmoothingMode` to control the output quality.  
4. Verify that PNG files are created alongside the original CMX files.

## Code Example
The following snippet demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "b68c26bbcad18022185d482650264be4" "CMXToPNGConversion.cs" >}}

## See Also
- **Converting CMX to JPEG** – learn how to produce JPEG outputs from CMX files.  
- **Working with Vector Rasterization Options** – explore additional rasterization settings available for vector formats.  
- **Batch image conversion with Aspose.Imaging** – process multiple image types in a single workflow.
