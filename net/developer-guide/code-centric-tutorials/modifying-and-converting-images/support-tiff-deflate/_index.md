---
title: Support TIFF Deflate Compression
linktitle: Support TIFF Deflate
type: docs
weight: 30
url: /net/support-tiff-deflate/
description: Demonstrates how to save a PNG with an alpha channel to a TIFF file using Deflate compression.
keywords: tiff deflate c#
---

# Support TIFF Deflate Compression

## Introduction
This example shows how to export a PNG image that contains an alpha channel to a TIFF file using the Deflate compression format. It is useful when you need lossless compression while preserving transparency in TIFF images.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample PNG image with an alpha channel (e.g., `sample.png`)

## Step-by-step Guide
1. Load the source PNG image using `Image.Load`.
2. Create a `TiffOptions` instance and set `TiffExpectedFormat` to `TiffDeflateRgba` to enable Deflate compression with RGBA support.
3. Save the image to a new TIFF file using the configured `TiffOptions`.
4. Verify the output file (`result.tiff`) contains the expected compressed data and alpha channel.

## Code Example
The following code demonstrates the process described above:

{{< gist "aspose-imaging-gists" "b13f8547b8725bbd26d11e64c2908d40" "SupportTiffDeflate.cs" >}}

## See Also
- Converting PNG to TIFF with LZW compression
- Working with TIFF metadata in Aspose.Imaging
- Modifying image pixel data before saving
