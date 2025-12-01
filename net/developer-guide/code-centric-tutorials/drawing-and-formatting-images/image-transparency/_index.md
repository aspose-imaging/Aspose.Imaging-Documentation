---
title: Working with Image Transparency in PNG Files
linktitle: Image Transparency
type: docs
weight: 30
url: /net/image-transparency/
description: Demonstrates how to read and assess image transparency (opacity) of a PNG image using Aspose.Imaging for .NET.
keywords: image transparency png c#
---

# Working with Image Transparency in PNG Files

## Introduction
This example shows how to load a PNG image and retrieve its opacity value, helping you determine whether the image is fully transparent, partially transparent, or opaque. Use it when you need to inspect or manipulate image transparency programmatically.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample PNG file (e.g., `sample.png`) placed in the example data folder

## Step-by-step Guide
1. Locate the directory that contains the sample PNG image.
2. Load the PNG image using `Image.Load`.
3. Cast the loaded image to `PngImage` to access PNG‑specific properties.
4. Retrieve the `ImageOpacity` property, which returns a floating‑point value between 0 (fully transparent) and 1 (fully opaque).
5. Evaluate the opacity value to determine the transparency state of the image.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "0c508510d6cfd2d5c4a3c5a45bbeae79" "Imagetransparency.cs" >}}

## See Also
- **Converting Images** – Learn how to convert PNG images to other formats with Aspose.Imaging.
- **Modifying Image Metadata** – Explore how to read and edit metadata of various image types.
- **Working with Image Layers** – Understand how to manipulate layers in multi‑layer image formats.
