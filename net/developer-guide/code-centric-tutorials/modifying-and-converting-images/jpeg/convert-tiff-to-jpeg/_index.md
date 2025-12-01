---
title: Convert TIFF Images to JPEG Format
linktitle: Convert TIFF to JPEG
type: docs
weight: 30
url: /net/convert-tiff-to-jpeg/
description: Demonstrates how to convert each frame of a multi-page TIFF file to JPEG while preserving resolution settings.
keywords: tiff jpeg conversion c#
---

# Convert TIFF Images to JPEG

## Introduction
This example shows how to load a multi‑page TIFF image, iterate through its frames, and save each frame as a JPEG file. It is useful when you need to extract individual pages from a TIFF document and retain the original resolution information.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample TIFF file (e.g., `source2.tif`) placed in the example data directory

## Step-by-step Guide
1. **Get the data directory** – Retrieve the path where example assets are stored.
2. **Load the TIFF image** – Use `Image.Load` to open the TIFF file as a `TiffImage`.
3. **Iterate through frames** – Loop over `tiffImage.Frames` to process each page.
4. **Configure JPEG options** – Create `JpegOptions`, copy the frame’s resolution, and set the appropriate resolution unit.
5. **Save each frame** – Generate a unique file name and call `tiffFrame.Save` with the JPEG options.
6. **Dispose resources** – The `using` statement ensures the TIFF image is properly released.

## Code Example
The complete example code is shown below:

{{< gist "aspose-imaging-gists" "53b02ad670195c1f0c03a2cb0ed81fd8" "ConvertTIFFToJPEG.cs" >}}

## See Also
- **Convert PNG to JPEG** – Learn how to change image formats while controlling compression.
- **Extract frames from a multi‑page TIFF** – Details on handling individual frames without conversion.
- **Adjust image resolution settings** – How to modify resolution metadata for various image formats.
