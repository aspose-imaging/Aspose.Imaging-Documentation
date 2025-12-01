---
title: Read and Write XMP Data to Images
linktitle: XMP Data
type: docs
weight: 30
url: /net/read-and-write-xmp-data-to-images/
description: Demonstrates how to embed and retrieve XMP metadata in TIFF images using Aspose.Imaging for .NET.
keywords: xmp, metadata, tiff
---

# Read and Write XMP Data to Images

## Introduction
This example shows how to add XMP metadata to a newly created TIFF image and then read it back. Use it when you need to embed rich information such as author, description, or Photoshop/Dublin Core data within image files.

## Prerequisites
- .NET 9.0 (or later)  
- Aspose.Imaging for .NET library  
- No additional files are required; the example creates its own image in memory.

## Step-by-step Guide
1. Create a TIFF image with the desired dimensions and format.  
2. Build an `XmpHeaderPi` and `XmpTrailerPi` to define the XMP packet.  
3. Populate an `XmpMeta` object with custom attributes (e.g., Author, Description).  
4. Add Photoshop and Dublin Core packages to enrich the metadata.  
5. Assign the assembled `XmpPacketWrapper` to the image’s `XmpData` property and save the image (to a stream or disk).  
6. Reload the image and access its `XmpData` to read back the stored metadata.

## Code Example
Below is the complete code for the scenario:

{{< gist "aspose-imaging-gists" "43eebf03ec07028adf45b293105b7cd1" "ReadAndWriteXMPDataToImages.cs" >}}

## See Also
- Adding EXIF metadata to images with Aspose.Imaging  
- Working with TIFF image frames in .NET  
- Converting between image formats using Aspose.Imaging
