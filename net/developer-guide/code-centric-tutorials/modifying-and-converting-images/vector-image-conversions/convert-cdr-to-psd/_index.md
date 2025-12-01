---
title: Convert CDR to PSD while Preserving Vector Shapes
linktitle: CDR to PSD conversion
type: docs
weight: 30
url: /net/convert-cdr-to-psd/
description: Export a CorelDRAW (CDR) file to PSD format preserving vector layers.
keywords: cdr psd conversion
---

# Convert CDR to PSD while Preserving Vector Shapes

## Introduction
This example demonstrates how to export a CorelDRAW (CDR) file to the Photoshop PSD format while keeping the original vector shapes intact. Use it when you need a PSD file that retains editable vector layers for further design work.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample CDR file (e.g., `SimpleShapes.cdr`) placed in the example data folder

## Step-by-step Guide
1. Load the CDR image using `Image.Load`.
2. Create a `PsdOptions` instance and configure its `VectorRasterizationOptions` to match the source image dimensions.
3. Set `VectorizationOptions` with `VectorDataCompositionMode.SeparateLayers` to keep vector shapes on separate PSD layers.
4. Save the image as a PSD file using the configured options.
5. (Optional) Delete the generated PSD file after verification.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "23e6877cffc6247e54359c40bbc46dcc" "ApsToPsd.cs" >}}

## See Also
- Export other vector formats (EMF, SVG, etc.) to PSD
- Working with PSD images in Aspose.Imaging
- Rasterizing vector images to bitmap formats
