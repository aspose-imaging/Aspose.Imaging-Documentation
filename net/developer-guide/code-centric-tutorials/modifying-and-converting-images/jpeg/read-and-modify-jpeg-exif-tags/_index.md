---
title: Read and Modify JPEG EXIF Tags
linktitle: Read and Modify JPEG EXIF Tags
type: docs
weight: 30
url: /net/read-and-modify-jpeg-exif-tags/
description: Demonstrates how to read and modify EXIF tags in a JPEG image using Aspose.Imaging for .NET.
keywords: exif jpeg c#
---

# Read and Modify JPEG EXIF Tags

## Introduction
This example shows how to load a JPEG image, access its EXIF metadata, enumerate all EXIF tags, and display their values. Use it when you need to inspect or manipulate image metadata in your .NET applications.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A JPEG file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Resolve the path to the folder that contains the sample JPEG image.  
2. Load the JPEG image using `Image.Load`.  
3. Cast the loaded image to `JpegImage` to obtain its `ExifData` property.  
4. Verify that EXIF metadata exists.  
5. Retrieve the type of the `ExifData` object and enumerate its public properties.  
6. For each property, read and output the property name and its current value.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "07a101161e184f9dd4517a6577f386e5" "ReadAndModifyJpegEXIFTags.cs" >}}

## See Also
- [Read and Write Image Metadata](/net/read-and-write-image-metadata/)
- [Convert JPEG to PNG](/net/convert-jpeg-to-png/)
- [Modify Image Resolution](/net/modify-image-resolution/)
