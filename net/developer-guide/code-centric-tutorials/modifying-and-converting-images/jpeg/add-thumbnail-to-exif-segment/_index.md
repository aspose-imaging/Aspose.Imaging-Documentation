---
title: Add a Thumbnail to an EXIF Segment in a JPEG Image
linktitle: Add Thumbnail to EXIF
type: docs
weight: 30
url: /net/add-thumbnail-to-exif-segment/
description: Demonstrates how to embed a thumbnail image into the EXIF segment of a JPEG file using Aspose.Imaging for .NET.
keywords: thumbnail exif jpeg
---

# Add a Thumbnail to an EXIF Segment in a JPEG Image

## Introduction
This example shows how to create a thumbnail image and embed it into the EXIF segment of a JPEG file. Use it when you need to enrich JPEG metadata with a preview image, such as for photo management or web display scenarios.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Access to a writable folder for output files

## Step-by-step Guide
1. Obtain the directory that contains your sample JPEG files.  
2. Create a small `JpegImage` that will serve as the thumbnail (e.g., 100 × 100 px).  
3. Load or create the main JPEG image you wish to modify.  
4. Initialize the `JpegExifData` for the main image if it is not already set.  
5. Assign the thumbnail image to the `ExifData.Thumbnail` property.  
6. Save the modified JPEG image to a new file, which now includes the embedded thumbnail.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "a7ebf30e57f960a190e52c2ff06f5c51" "AddThumbnailToEXIFSegment.cs" >}}

## See Also
- [Working with EXIF Data in JPEG Images](#)
- [Creating and Saving JPEG Images with Aspose.Imaging](#)
- [Modifying Image Metadata Using Aspose.Imaging for .NET](#)
