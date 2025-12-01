---
title: Export Metafile to Multiple Raster Formats
linktitle: Export Metafile to Raster Formats
type: docs
weight: 30
url: /net/export-meta-file-to-raster-formats/
description: Demonstrates how to export an EMF metafile to various raster image formats using Aspose.Imaging for .NET.
keywords: emf, raster, convert c#
---

# Export Metafile to Multiple Raster Formats

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image and export it to several common raster formats such as BMP, GIF, JPEG, PNG, TIFF, and WebP. Use it when you need to convert vector‑based metafiles into raster images for broader compatibility or downstream processing.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An EMF file (e.g., `Picture1.emf`) placed in the example data directory

## Step-by-step Guide
1. **Prepare the output path** – Define a base file name for the generated images.  
2. **Configure rasterization options** – Create an `EmfRasterizationOptions` instance and set properties such as background color, page width, and page height.  
3. **Load the EMF file** – Use `Image.Load` to read the metafile and cast it to `EmfImage`.  
4. **Validate the EMF header** – Ensure the file is a valid EMF before proceeding.  
5. **Save to each raster format** – Call `image.Save` with the appropriate `*Options` (e.g., `BmpOptions`, `JpegOptions`, `PngOptions`, etc.) while passing the rasterization options.  
6. **Dispose resources** – The `using` statement automatically releases the image resources after conversion.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b092d582240c111d602e06c47c70c730" "ExportMetaFileToRasterFormats.cs" >}}

## See Also
- Export Metafile to Vector Formats  
- Convert PDF to Raster Images  
- Manipulating Image Color Profiles
