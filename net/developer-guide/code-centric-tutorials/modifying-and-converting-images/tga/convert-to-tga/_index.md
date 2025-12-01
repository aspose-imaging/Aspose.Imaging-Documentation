---
title: Convert JPEG and PNG Images to TGA Using Aspose.Imaging
linktitle: Convert to TGA
type: docs
weight: 30
url: /net/convert-to-tga/
description: Demonstrates how to convert JPEG and PNG images to TGA format and modify TGA metadata with Aspose.Imaging for .NET.
keywords: tga conversion c#
---

# Convert JPEG and PNG Images to TGA Format

## Introduction
This example shows how to load JPEG and PNG images, convert them to the TGA format, and edit various metadata fields of an existing TGA image. Use it when you need lossless TGA output or want to embed custom information such as author name, timestamps, or software details.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library
- Sample image files: `test.jpg`, `test.png`, and `test.tga` placed in the data directory used by the example

## Step-by-step Guide
1. **Prepare the input files** – locate the source JPEG, PNG, and TGA images in the data directory.  
2. **Load a JPEG image** using `Image.Load` and cast it to `RasterImage`.  
3. **Save the JPEG as TGA** by calling `image.Save` with a new `TgaOptions` instance.  
4. **Load a PNG image**, convert it to a `TgaImage` via the `TgaImage` constructor, and save it.  
5. **Load an existing TGA image** and modify its metadata fields (e.g., `DateTimeStamp`, `AuthorName`, `TransparentColor`, etc.).  
6. **Save the updated TGA image** back to disk.  
7. **Clean up** – delete the generated TGA files after verification.

## Code Example
The full source code for this example is shown below:

{{< gist "aspose-imaging-gists" "6c283fd369e368281b92cb05c2973dee" "ConvertToTGA.cs" >}}

## See Also
- **Convert BMP to TGA** – Learn how to convert bitmap images to the TGA format.  
- **Modify TGA Metadata** – Detailed guide on editing additional TGA header fields.  
- **Working with Raster Images** – Overview of raster image manipulation using Aspose.Imaging.
