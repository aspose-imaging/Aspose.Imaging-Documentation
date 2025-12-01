---
title: Export Image to Different Formats
linktitle: Export Image Formats
type: docs
weight: 30
url: /net/export-image-to-different-formats/
description: Demonstrates how to export a GIF image to BMP, JPEG, PNG, and TIFF using Aspose.Imaging for .NET.
keywords: export image format c#
---

# Export Image to Different Formats

## Introduction
This example shows how to load a GIF image and export it to several popular raster formats—BMP, JPEG, PNG, and TIFF—using Aspose.Imaging for .NET. It is useful when you need to generate multiple output types from a single source image.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample GIF file (e.g., `sample.gif`) placed in the data directory used by the example

## Step-by-step Guide
1. **Prepare the data directory** – Obtain the folder that contains `sample.gif` and where the exported files will be saved.  
2. **Load the source image** – Use `Image.Load` to read the GIF file into an `Image` object.  
3. **Export to BMP** – Call `image.Save` with a `BmpOptions` instance and specify the output file name (`_output.bmp`).  
4. **Export to JPEG** – Call `image.Save` with a `JpegOptions` instance and specify the output file name (`_output.jpeg`).  
5. **Export to PNG** – Call `image.Save` with a `PngOptions` instance and specify the output file name (`_output.png`).  
6. **Export to TIFF** – Call `image.Save` with a `TiffOptions` instance (using `TiffExpectedFormat.Default`) and specify the output file name (`_output.tiff`).  
7. **Dispose the image** – The `using` block ensures the image resources are released automatically.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "f65dd860929453bdde4a188fc2c0c96c" "ExportImageToDifferentFormats.cs" >}}

## See Also
- **Loading and Saving Images** – Learn how to load different image formats and save them after processing.  
- **Applying Image Options** – Explore how to customize output files using various image options (e.g., compression, quality).  
- **Converting Image Formats** – A broader guide on converting images between formats with Aspose.Imaging.
