---
title: Read Pixel Values from a TIFF Image using Aspose.Imaging for .NET
linktitle: Read Pixel Values
type: docs
weight: 30
url: /net/reading-pixel-values/
description: Demonstrates how to load a TIFF image and read ARGB pixel values with Aspose.Imaging for .NET.
keywords: read pixel values c#
---

# Read Pixel Values from a TIFF Image

## Introduction
This example shows how to load a 16‑bit TIFF image, extract its ARGB pixel data, and print the individual channel values. Use it when you need to inspect raw pixel information or perform custom analyses on high‑depth images.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample 16‑bit uncompressed TIFF file (as used in the example)

## Step-by-step Guide
1. **Set the data directory** – Obtain the folder that contains the sample image.
2. **Create `LoadOptions`** – Disable ICC profile conversion for 16‑bit images.
3. **Define the region of interest** – Specify a rectangle that bounds the pixels you want to read.
4. **Load the image as `RasterImage`** using `Image.Load` with the prepared `LoadOptions`.
5. **Retrieve ARGB64 pixel data** with `LoadArgb64Pixels`.
6. **Iterate through the selected rectangle** and decode the 64‑bit color values into alpha, red, green, and blue components.
7. **Output the channel values** – Write the extracted values to the console or desired destination.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "17502b20b4ee259f26a11ce3c4c07b98" "ReadingPixelVaules.cs" >}}

## See Also
- **Converting Image Formats** – Learn how to convert images between different file types with Aspose.Imaging.
- **Manipulating Image Metadata** – Explore how to read and modify image metadata such as EXIF and ICC profiles.
- **Working with High‑Depth Images** – Guidelines for processing 16‑bit and higher color depth images.
