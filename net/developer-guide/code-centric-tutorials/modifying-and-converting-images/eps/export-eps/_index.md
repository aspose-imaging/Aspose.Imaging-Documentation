---
title: Export EPS Image Preview
linktitle: Export EPS
type: docs
weight: 30
url: /net/export-eps/
description: Demonstrates how to generate a TIFF preview image from an EPS file using Aspose.Imaging for .NET.
keywords: eps preview, tiff, c#
---

# Export EPS Image Preview

## Introduction
This example shows how to load an EPS file and create a TIFF preview image from it. Use this approach when you need a quick raster representation of vector EPS content, for thumbnails or for further raster processing.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample EPS file (e.g., `Sample.eps`) placed in the data directory used by the examples

## Step-by-step Guide
1. Obtain the path to the folder that contains the EPS sample file.  
2. Load the EPS file with `Image.Load` and cast it to `EpsImage`.  
3. Call `GetPreviewImage(EpsPreviewFormat.TIFF)` to generate a preview image in TIFF format.  
4. If the preview image is not null, save it to a memory stream or directly to a file.  
5. Dispose of the image and any streams after use to free resources.

## Code Example
The following code snippet implements the steps described above:

{{< gist "aspose-imaging-gists" "0ccd6d3c8fe3cc5722ba97c44381fb3c" "ExportEps.cs" >}}

## See Also
- **Convert EPS to PDF** – Learn how to convert EPS files directly to PDF format.  
- **Export EPS to PNG** – Generate PNG raster images from EPS files.  
- **Working with TIFF Images** – Explore additional TIFF image processing capabilities in Aspose.Imaging.
