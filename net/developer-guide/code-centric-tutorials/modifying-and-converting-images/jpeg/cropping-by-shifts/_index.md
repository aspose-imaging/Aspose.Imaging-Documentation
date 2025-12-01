---
title: Crop JPEG Images Using Shift Values
linktitle: Cropping by Shifts
type: docs
weight: 30
url: /net/cropping-by-shifts/
description: Demonstrates how to crop a JPEG image by specifying shift values for each side using Aspose.Imaging for .NET.
keywords: crop jpeg c#
---

# Crop JPEG Images Using Shift Values

## Introduction
This example shows how to crop a JPEG image by providing shift values for the left, right, top, and bottom edges. It is useful when you need to trim a picture uniformly from all sides without calculating exact pixel coordinates.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A JPEG file to work with (e.g., `aspose-logo.jpg`)

## Step-by-step Guide
1. **Load the source JPEG** – Use `Image.Load` to read the image into a `RasterImage` instance.  
2. **Cache the image (optional)** – Call `CacheData` if the image is not already cached for better performance.  
3. **Define shift values** – Set integer values for `leftShift`, `rightShift`, `topShift`, and `bottomShift`.  
4. **Crop the image** – Invoke `RasterImage.Crop(leftShift, rightShift, topShift, bottomShift)` to apply the shifts.  
5. **Save the result** – Call `Save` to write the cropped image to a new file.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "13b21eaa923dca59c13c6e7f36491894" "CroppingByShifts.cs" >}}

## See Also
- Resizing JPEG Images  
- Rotating Images  
- Saving Images in Different Formats
