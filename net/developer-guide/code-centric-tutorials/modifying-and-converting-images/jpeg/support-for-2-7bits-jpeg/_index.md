---
title: Support for 2‑7 Bits JPEG Compression
linktitle: Support for 2‑7 Bits JPEG
type: docs
weight: 30
url: /net/support-for-2-7bits-jpeg/
description: Demonstrates how to save a PNG image as JPEG‑LS with reduced bits per channel using Aspose.Imaging for .NET.
keywords: jpeg ls c#
---

# Support for 2‑7 Bits JPEG Compression

## Introduction
This example shows how to convert a PNG image to JPEG‑LS while specifying a lower bits‑per‑channel value (2 bits). Reducing the bits per sample can significantly lower the file size, which is useful when bandwidth or storage is limited. Use this technique when you need lossy compression with fine‑grained control over image quality.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A source PNG image (e.g., `lena_16g_lin.png`) placed in the example data folder

## Step-by-step Guide
1. Locate the directory containing the source PNG image using `RunExamples.GetDataDir_JPEG()`.
2. Define the desired bits per channel (e.g., `int bpp = 2;` for 2‑bit samples).
3. Load the source PNG image with `PngImage`.
4. Create a `JpegOptions` instance, set `BitsPerChannel` to the desired value, and select `JpegCompressionMode.JpegLs`.
5. Save the image as a JPEG‑LS file using the configured options.
6. To verify the result, load the generated JPEG‑LS file and save it back to PNG format for visual inspection.

## Code Example
The following code demonstrates the process:

{{< gist "aspose-imaging-gists" "04c10a624c6c975ba80f44efa0792856" "SupportFor2-7BitsJPEG.cs" >}}

## See Also
- Converting PNG to JPEG with Aspose.Imaging  
- Working with JPEG‑LS images in .NET  
- Adjusting image bit depth and compression settings
