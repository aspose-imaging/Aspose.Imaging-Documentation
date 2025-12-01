---
title: Export JPEG and Multi‑page Images to DICOM Format
linktitle: Export to DICOM
type: docs
weight: 30
url: /net/export-to-dicom/
description: Convert JPEG or multi‑page TIFF/GIF images to DICOM using Aspose.Imaging for .NET.
keywords: dicom, convert, c#
---

# Export JPEG and Multi‑page Images to DICOM Format

## Introduction
This example demonstrates how to convert a single‑page JPEG image and a multi‑page TIFF (or GIF) image into the DICOM file format. Use it when you need to generate DICOM files from standard image sources for medical imaging workflows.

## Prerequisites
- .NET 9.0 (or later compatible version)
- Aspose.Imaging for .NET library
- Sample image files: `sample.jpg` and `multipage.tif` located in the example data directory

## Step-by-step Guide
1. **Prepare the input files** – Locate the JPEG and multi‑page TIFF/GIF files in the data directory.
2. **Load the image** – Use `Image.Load` to read each file into an `Image` object.
3. **Save as DICOM** – Call `image.Save` with a `DicomOptions` instance to write the output `.dcm` files.
4. **Repeat for multi‑page images** – The same approach works for GIF or TIFF files containing multiple frames.

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "83092ab6efd5f4cb094f922bcfddf066" "ExportToDicom.cs" >}}

## See Also
- Converting Images to PDF Format
- Working with Multi‑page TIFF Images
- Exporting Images to DICOM Series in Aspose.Imaging
