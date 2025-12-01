---
title: Support for CMYK and YCCK Color Modes in JPEG Lossless Using RGB Profile
linktitle: CMYK/YCCK JPEG Lossless
type: docs
weight: 30
url: /net/support-for-cmyk-and-ycck-color-modes-in-jpeg-lossless-using-rgb-profile/
description: Demonstrates how to save and load JPEG lossless images with CMYK/YCCK color modes using custom RGB and CMYK profiles.
keywords: cmyk jpeg .net
---

# Support for CMYK and YCCK Color Modes in JPEG Lossless Using RGB Profile

## Introduction
This example shows how to work with JPEG images that use CMYK or YCCK color modes in a lossless compression scenario. It demonstrates saving a JPEG with custom RGB and CMYK ICC profiles and then loading it back while preserving those profiles. Use this when you need precise color management for professional printing workflows.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Input files: `056.jpg`, `eciRGB_v2.icc`, `ISOcoated_v2_FullGamut4.icc`

## Step-by-step Guide
1. **Prepare source streams** – Open file streams for the RGB and CMYK ICC profile files and wrap them in `Sources.StreamSource` objects.  
2. **Load the JPEG image** – Use `Image.Load` to load the source JPEG (`056.jpg`) as a `JpegImage`.  
3. **Configure JPEG options** – Create a `JpegOptions` instance, set `ColorType` to `Cmyk`, set `CompressionType` to `Lossless`, and assign the custom `RgbColorProfile` and `CmykColorProfile`.  
4. **Save to a memory stream** – Save the image to a `MemoryStream` using the configured `JpegOptions`.  
5. **Reload from the memory stream** – Reset the stream position, then load the image back from the stream.  
6. **Assign profiles after loading** – Set `RgbColorProfile` and `CmykColorProfile` on the loaded image to ensure the correct color interpretation.  
7. **Export to another format** – Save the image as a PNG (or any other supported format) using appropriate options such as `PngOptions`.  
8. **Dispose resources** – Ensure all streams and images are properly disposed to release file handles.

## Code Example
The following code illustrates the complete process:

{{< gist "aspose-imaging-gists" "249092b937c32fbb051170324e39a070" "SupportForCMYKAndYCCKColorModesInJPEGLosslessUsingRGBProfile.cs" >}}

## See Also
- Working with JPEG images in Aspose.Imaging
- Converting JPEG to PNG using Aspose.Imaging
- Managing ICC color profiles in .NET applications
