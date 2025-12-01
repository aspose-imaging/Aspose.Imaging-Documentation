---
title: Support for CMYK and YCCK Color Modes in JPEG Lossless
linktitle: CMYK/YCCK JPEG Lossless
type: docs
weight: 30
url: /net/support-for-cmyk-and-ycck-color-modes-in-jpeg-lossless/
description: Demonstrates how to save and load JPEG images using CMYK and YCCK color modes with lossless compression.
keywords: jpeg cmyk .net
---

# Support for CMYK and YCCK Color Modes in JPEG Lossless

## Introduction
This example shows how to work with JPEG images that use CMYK and YCCK color spaces while applying lossless compression. Use it when you need to preserve color fidelity in professional printing workflows or when handling images that originate from CMYK sources.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample JPEG file (e.g., `056.jpg`) placed in the data directory

## Step-by-step Guide
1. Load the source JPEG image using `JpegImage`.
2. Configure `JpegOptions` with `ColorType` set to `JpegCompressionColorMode.Cmyk` and `CompressionType` set to `JpegCompressionMode.Lossless`.
3. Save the image to a memory stream with the configured options.
4. Reset the stream position and reload the JPEG image from the stream.
5. Export the loaded image to another format (e.g., PNG) to verify the conversion.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "fed2f59a3e17d131b5d67720a66aea1d" "SupportForCMYKAndYCCKColorModesInJPEGLossless.cs" >}}

## See Also
- Converting JPEG images to other formats
- Working with color profiles in Aspose.Imaging
- Lossless image compression techniques
