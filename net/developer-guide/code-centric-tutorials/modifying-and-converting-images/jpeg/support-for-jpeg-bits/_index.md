---
title: Using JPEG‑LS with 2 Bits per Sample (Support for JPEG‑BITS)
linktitle: Support for JPEG‑BITS
type: docs
weight: 10
url: /net/support-for-jpeg-bits/
description: Demonstrates how to save a PNG as JPEG‑LS with reduced bits per channel and convert it back to PNG using Aspose.Imaging for .NET.
keywords: jpeg ls c#
---

# Using JPEG‑LS with 2 Bits per Sample (Support for JPEG‑BITS)

## Introduction
This example shows how to convert a high‑bit‑depth PNG image to a JPEG‑LS image using only 2 bits per channel, then convert the JPEG‑LS back to PNG for visual verification. It is useful when you need to reduce file size while preserving acceptable visual quality.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample PNG image (e.g., `lena_16g_lin.png`) placed in the example data folder

## Step-by-step Guide
1. **Prepare the source PNG** – Retrieve the full‑color PNG file from the data directory.
2. **Create JPEG‑LS options** – Instantiate `JpegOptions`, set `BitsPerChannel` to `2`, and choose `JpegCompressionMode.JpegLs`.
3. **Convert PNG to JPEG‑LS** – Load the PNG with `PngImage`, then call `Save` using the configured `JpegOptions`.
4. **Convert back to PNG** – Load the generated JPEG‑LS with `JpegImage` and save it as a PNG using `PngOptions` for visual inspection.
5. **Verify the output** – Compare the sizes and visual quality of the original PNG, the compressed JPEG‑LS, and the reconverted PNG.

## Code Example
The following gist contains the complete C# implementation of the steps described above:

{{< gist "aspose-imaging-gists" "f1bf21502e0a32b762837d0d529f595a" "SupportForJPEG.cs" >}}

## See Also
- [Saving Images in Different Formats with Aspose.Imaging for .NET](./saving-images-in-different-formats)
- [Adjusting Image Quality and Compression Settings](./adjusting-image-quality)
- [Working with PNG Images Using Aspose.Imaging](./png-image-manipulation)
