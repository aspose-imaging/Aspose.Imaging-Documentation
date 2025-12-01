---
title: Rotate a JPEG Image Using Aspose.Imaging for .NET
linktitle: Rotate JPEG Image
type: docs
weight: 30
url: /net/rotating-an-image/
description: Demonstrates how to rotate a JPEG image by 270° using Aspose.Imaging for .NET.
keywords: rotate image c# jpeg
---

# Rotate a JPEG Image Using Aspose.Imaging for .NET

## Introduction
This example shows how to load a JPEG image, rotate it by 270 degrees, and save the result. Use it when you need to adjust image orientation programmatically within a .NET application.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A JPEG file (e.g., `aspose-logo.jpg`) placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the source JPEG image.
2. Load the image using `Image.Load`.
3. Call `RotateFlip` with `RotateFlipType.Rotate270FlipNone` to rotate the image.
4. Save the rotated image to a new file using `image.Save`.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "e30585ccae6e06456c5dd04a0cc139eb" "RotatingAnImage.cs" >}}

## See Also
- [Resize a JPEG Image](#)  
- [Convert JPEG to PNG](#)  
- [Apply Watermark to an Image](#)
