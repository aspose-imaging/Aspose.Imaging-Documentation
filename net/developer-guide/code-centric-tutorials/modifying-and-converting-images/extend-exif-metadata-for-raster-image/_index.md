---
title: Extend EXIF Metadata for Raster Images
linktitle: Extend EXIF Metadata
type: docs
weight: 30
url: /net/extend-exif-metadata-for-raster-image/
description: Demonstrates how to add or modify EXIF and XMP metadata in raster images using Aspose.Imaging for .NET.
keywords: exif metadata c#
---

# Extend EXIF Metadata for Raster Images

## Introduction
This example shows how to extend or modify EXIF and XMP metadata embedded in raster images such as PNG files. Use it when you need to enrich images with custom metadata or adjust existing orientation information.

## Prerequisites
- .NET 5.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- A sample raster image file (e.g., PNG) placed in the data folder used by the example

## Step-by-step Guide
1. Load the raster image using `Image.Load`.
2. Check if the image contains XMP data; if so, create a new `XmpBasicPackage` and add custom key‑value pairs.
3. Append the new XMP package to the image’s `XmpData`.
4. If the image contains EXIF data, modify the desired EXIF fields (e.g., set `Orientation`).
5. Save the image to a temporary output file.
6. (Optional) Delete the temporary file to clean up after verification.

## Code Example
The full source code for this scenario is provided below:

{{< gist "aspose-imaging-gists" "9821184a2b609953bb39cde7e2eadfa6" "ExtendExifMetadataForRasterImage.cs" >}}

## See Also
- Working with EXIF data in Aspose.Imaging
- Exporting image metadata to other formats
- Overwriting image metadata with custom profiles
