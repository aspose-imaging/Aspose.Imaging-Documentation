---
title: Support of GetOriginalOptions in TIFF Images
linktitle: GetOriginalOptions (TIFF)
type: docs
weight: 30
url: /net/support-of-get-original-options/
description: Demonstrates how to use GetOriginalOptions to preserve original TIFF data when saving images.
keywords: tiff getoriginaloptions c#
---

# Support of GetOriginalOptions in TIFF Images

## Introduction
This example shows how to employ the **GetOriginalOptions** method to retain the original TIFF image data during saving operations. Use it when you need to create copies of a TIFF file without altering its compression or metadata.

## Prerequisites
- .NET 6.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- A TIFF source file (e.g., `lichee.tif`) placed in the data directory used by the examples

## Step-by-step Guide
1. Load the source TIFF image using `Image.Load`.
2. Call `image.GetOriginalOptions()` and pass the returned options to `image.Save` to create a copy that preserves the original format.
3. For a specific frame, cast the image to `TiffImage`, retrieve the desired `TiffFrame`, and use `frame.GetOriginalOptions()` when saving the frame.
4. Clean up any temporary files created during the process.

## Code Example
The following code demonstrates the workflow described above:

{{< gist "aspose-imaging-gists" "6ce9e832007bd5be548087d0e922e8ca" "SupportOfGetOriginalOptions.cs" >}}

## See Also
- Working with TIFF Images in Aspose.Imaging
- Saving Images with Original Options
- Modifying Image Frames in TIFF Files
