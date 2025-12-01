---
title: Convert CDR to PNG with Aspose.Imaging for .NET
linktitle: CDR to PNG
type: docs
weight: 30
url: /net/cdr-to-png/
description: Demonstrates how to load a CDR file and save it as a PNG image using Aspose.Imaging for .NET.
keywords: cdr png conversion
---

# Convert CDR to PNG

## Introduction
This example shows how to load a CorelDRAW (CDR) file, configure PNG export options, and save the result as a PNG image. It is useful when you need to rasterize vector drawings from CDR files for web or application use.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- An example CDR file (e.g., `SimpleShapes.cdr`) placed in the data directory used by the sample

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path where the sample CDR file resides.
2. **Load the CDR image** – Use `Image.Load` to open the CDR file as a `CdrImage`.
3. **Create PNG options** – Instantiate `PngOptions` and set the desired color type (Truecolor with Alpha).
4. **Configure rasterization** – Obtain default rasterization options from the loaded CDR image and adjust text rendering hint and smoothing mode.
5. **Save as PNG** – Call `image.Save` with the target PNG file name and the configured options.
6. **Clean up** – Optionally delete the generated PNG file after verification.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "97c27f49b6ad752ce7c40442abad5f57" "CdrToPngExample.cs" >}}

## See Also
- Converting other vector formats (SVG, WMF) to raster images
- Working with `PngOptions` for fine‑tuned PNG output
- General image loading and saving with Aspose.Imaging for .NET
