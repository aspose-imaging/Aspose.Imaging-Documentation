---
title: Compress DICOM Images with Various Algorithms using Aspose.Imaging for .NET
linktitle: DICOM Compression
type: docs
weight: 30
url: /net/dicom-compression/
description: Demonstrates how to compress DICOM images using different compression types with Aspose.Imaging for .NET.
keywords: dicom compression c#
---

# Compress DICOM Images with Various Algorithms

## Introduction
This example shows how to load a standard image, convert it to the DICOM format, and apply several compression methods such as None, JPEG, JPEG2000, and RLE. Use it when you need to generate DICOM files with specific compression requirements for medical imaging workflows.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A source image file (e.g., `original.jpg`) placed in the example data folder

## Step-by-step Guide
1. **Load the source image** using `Image.Load`.
2. **Create a `DicomOptions` instance** and set:
   - `ColorType` to `Rgb24Bit`
   - Desired `Compression` type (`None`, `Jpeg`, `Jpeg2000`, or `Rle`).
3. **Save the image** to a `.dcm` file with the configured options.
4. **Repeat steps 2‑3** for each compression type you want to generate.
5. **Clean up** by deleting the generated DICOM files if they are only needed for demonstration.

## Code Example
The complete source code for this example is shown below:

{{< gist "aspose-imaging-gists" "da5be1210da6641be6bb539d2fb6cfd7" "DicomCompression.cs" >}}

## See Also
- Working with DICOM images in Aspose.Imaging
- Saving images in JPEG2000 format
- Applying image compression with Aspose.Imaging for .NET
