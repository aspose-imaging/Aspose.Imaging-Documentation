---
title: Write and Modify EXIF Data in JPEG Images
linktitle: Write/Modify EXIF Data
type: docs
weight: 30
url: /net/writing-and-modifying-exif-data/
description: Demonstrates how to read and update EXIF metadata in a JPEG image using Aspose.Imaging for .NET.
keywords: exif jpeg c#
---

# Write and Modify EXIF Data in JPEG Images

## Introduction
This example shows how to load a JPEG image, read its existing EXIF metadata, modify fields such as LensMake, WhiteBalance, and Flash, and then save the updated image. Use it when you need to programmatically adjust EXIF information for photography or imaging workflows.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample JPEG file (e.g., `aspose-logo.jpg`) placed in the data directory used by the example

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder that contains the input JPEG file.  
2. **Load the JPEG image** – Use `Image.Load` to open the image as a `JpegImage`.  
3. **Access EXIF data** – Retrieve the `JpegExifData` object via the `ExifData` property.  
4. **Modify EXIF fields** – Assign new values to properties such as `LensMake`, `WhiteBalance`, and `Flash`.  
5. **Save the updated image** – Call `image.Save` with a new file name to persist the changes.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "46619f88283b4b66448988a3515952fa" "WritingAndModifyingEXIFData.cs" >}}

## See Also
- **Reading EXIF Data from JPEG Images** – learn how to extract EXIF metadata without altering it.  
- **Converting JPEG to PNG** – discover how to change the image format while preserving visual quality.  
- **Batch Processing Multiple Images** – apply EXIF modifications across a collection of files in one operation.
