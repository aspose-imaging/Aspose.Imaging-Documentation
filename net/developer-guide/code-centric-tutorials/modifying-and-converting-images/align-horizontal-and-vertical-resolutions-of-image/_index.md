---
title: Align Horizontal and Vertical Resolutions of an Image
linktitle: Align Resolutions
type: docs
weight: 30
url: /net/align-horizontal-and-vertical-resolutions-of-image/
description: Aligns the horizontal and vertical resolutions of a TIFF image so they are equal.
keywords: tiff align resolution c#
---

# Align Horizontal and Vertical Resolutions of an Image

## Introduction
This example demonstrates how to align the horizontal and vertical resolutions of a TIFF image using Aspose.Imaging for .NET. Aligning resolutions is useful when you need consistent DPI values across both axes, which can simplify further image processing or printing tasks.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample TIFF image (e.g., `SampleTiff1.tiff`) placed in the examples data folder

## Step-by-step Guide
1. **Load the TIFF image** – Use `Image.Load` to read the image file and cast it to `TiffImage`.
2. **Call AlignResolutions** – Invoke `image.AlignResolutions()` to make the horizontal and vertical DPI values equal.
3. **Save the result** – Save the modified image to a new file, typically with an `_out.tiff` suffix.
4. **Verify the alignment** – Iterate through the image frames (if multi‑frame) and confirm that `HorizontalResolution` matches `VerticalResolution`.

## Code Example
The following code snippet shows the complete workflow:

{{< gist "aspose-imaging-gists" "f1ea71fe314f0c42b7a9368f9ca43a2d" "AlignHorizontalAndVeticalResolutionsOfImage.cs" >}}

## See Also
- **Changing Image DPI** – Learn how to set a specific DPI for an image.
- **Converting TIFF to Other Formats** – Example of converting a TIFF image to JPEG or PNG.
- **Working with Multi‑page TIFFs** – How to manipulate individual frames within a multi‑page TIFF file.
