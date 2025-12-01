---
title: Configuring TIFF Options in Aspose.Imaging for .NET
linktitle: TIFF Options Configuration
type: docs
weight: 30
url: /net/tiff-options-configuration/
description: Demonstrates how to set TIFF compression and color format using TiffOptions.
keywords: tiff options c# imaging
---

# Configuring TIFF Options

## Introduction
This example shows how to configure TIFF image saving options with Aspose.Imaging for .NET. It illustrates setting the compression format to JPEG and ensuring the image uses the RGB color space. Use this when you need to create optimized TIFF files for storage or web delivery.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample TIFF file (e.g., `SampleTiff1.tiff`) placed in the project’s data directory

## Step-by-step Guide
1. **Prepare the data directory** – Resolve the path where the sample TIFF resides.
2. **Load the source image** – Use `Image.Load` to read the TIFF file into an `Image` object.
3. **Create `TiffOptions`** – Instantiate `TiffOptions` with `TiffExpectedFormat.TiffJpegRgb` to specify JPEG compression and RGB color depth.
4. **Save the image** – Call `image.Save` with the desired output path and the configured `TiffOptions`.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "53b55547ad223dd2e830082deb846fb1" "TiffOptionsConfiguration.cs" >}}

## See Also
- Converting images to different formats with Aspose.Imaging
- Controlling image compression settings
- Working with other TIFF-specific options such as multi-page TIFF handling
