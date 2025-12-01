---
title: Auto-correct Orientation of JPEG Images
linktitle: Auto-correct JPEG Orientation
type: docs
weight: 30
url: /net/auto-correct-orientation-of-jpeg-images/
description: Demonstrates how to automatically rotate JPEG images based on EXIF orientation data using Aspose.Imaging for .NET.
keywords: jpeg orientation c#
---

# Auto-correct Orientation of JPEG Images

## Introduction
This example shows how to automatically adjust the rotation of a JPEG image according to the orientation information stored in its EXIF metadata. Use it when you need to ensure that JPEG images display correctly regardless of how they were captured.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample JPEG image (e.g., `aspose-logo.jpg`) placed in the data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the source JPEG image.  
2. Load the image using `Image.Load` and cast it to `JpegImage`.  
3. Call the `AutoRotate()` method on the `JpegImage` instance to apply the correct orientation based on EXIF data.  
4. Save the rotated image to a new file (for example, `aspose-logo_out.jpg`).  

## Code Example
The following code demonstrates how to auto‑rotate a JPEG image based on its EXIF orientation data.

{{< gist "aspose-imaging-gists" "3c4ae6091f4d58bac5fe7de4918f1f5f" "AutoCorrectOrientationOfJPEGImages.cs" >}}

## See Also
- Converting JPEG images to other formats with Aspose.Imaging
- Removing EXIF metadata from images
- Adjusting JPEG image quality using Aspose.Imaging
