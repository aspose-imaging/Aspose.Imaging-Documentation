---
title: Read Specific EXIF Tags Information
linktitle: Read EXIF Tags
type: docs
weight: 30
url: /net/read-specific-exif-tags-information/
description: Demonstrates how to extract selected EXIF metadata from a JPEG image using Aspose.Imaging for .NET.
keywords: exif jpeg c#
---

# Read Specific EXIF Tags Information

## Introduction
This example shows how to load a JPEG image and retrieve a few selected EXIF tags such as WhiteBalance, Pixel dimensions, ISO speed, and FocalLength. Use it when you need to inspect image metadata without processing the entire image.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- Sample JPEG file (e.g., `aspose-logo.jpg`) placed in the project data directory

## Step-by-step Guide
1. Obtain the path to the folder that contains the sample JPEG image.  
2. Load the JPEG image using `Image.Load`.  
3. Cast the loaded image to `JpegImage` and access its `ExifData` property.  
4. Verify that EXIF data is available.  
5. Read and display the desired EXIF properties (`WhiteBalance`, `PixelXDimension`, `PixelYDimension`, `ISOSpeed`, `FocalLength`).  

## Code Example
The following code demonstrates how to read specific EXIF tags from a JPEG image:

{{< gist "aspose-imaging-gists" "3b9fe73cb103afc39ab51f1154ee1b58" "ReadSpecificEXIFTagsInformation.cs" >}}

## See Also
- [Reading All EXIF Data from an Image](#)
- [Modifying EXIF Tags in a JPEG Image](#)
- [Converting JPEG to PNG Using Aspose.Imaging](#)
