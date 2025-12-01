---
title: Deskew an Image using Aspose.Imaging for .NET
linktitle: Deskew Image
type: docs
weight: 30
url: /net/deskew/
description: Removes skew from a scanned image using Aspose.Imaging for .NET.
keywords: deskew image c#
---

# Deskew an Image

## Introduction
This example demonstrates how to automatically remove the skew from a scanned image. Use it when you need to straighten scanned documents or photographs that were captured at an angle.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A skewed PNG image file (e.g., `skewed.png`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder that contains the example data files.
2. Load the skewed image using `Image.Load`.
3. Call `NormalizeAngle` on the loaded `RasterImage` to correct the tilt.
4. Save the corrected image to a new file.
5. Verify the output image has been deskewed.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "aaeed86fab81ec6ab045ad9c227a62e3" "Deskew.cs" >}}

## See Also
- Normalize image angle using Aspose.Imaging
- Rotate and flip images programmatically
- Convert image formats with Aspose.Imaging
