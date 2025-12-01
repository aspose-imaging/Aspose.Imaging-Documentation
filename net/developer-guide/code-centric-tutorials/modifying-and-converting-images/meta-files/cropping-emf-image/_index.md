---
title: Crop an EMF Image and Save as PDF
linktitle: Crop EMF Image
type: docs
weight: 30
url: /net/cropping-emf-image/
description: Demonstrates how to crop an EMF image and save it as a PDF using Aspose.Imaging for .NET.
keywords: crop emf pdf
---

# Crop an EMF Image and Save as PDF

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image, apply cropping by shifting its bounds, and then save the result as a PDF document. Use it when you need to trim vector graphics before rasterizing them to PDF.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input file: `Picture1.emf` placed in the example data directory

## Step-by-step Guide
1. **Set up rasterization options** – Create an `EmfRasterizationOptions` object and configure background color.
2. **Configure PDF options** – Assign the rasterization options to a `PdfOptions` instance.
3. **Load the EMF image** – Use `Image.Load` to load `Picture1.emf` as an `EmfImage`.
4. **Crop the image** – Call `image.Crop(left, top, right, bottom)` with the desired shift values (e.g., 30, 40, 50, 60).
5. **Adjust page size** – Set `PageWidth` and `PageHeight` of the rasterization options to match the cropped image dimensions.
6. **Save as PDF** – Invoke `image.Save(outputStream, pdfOptions)` to write the cropped image to a PDF file.

## Code Example
The following snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "d4f913a811c8e1a318eeb2359a448921" "CroppingEMFImage.cs" >}}

## See Also
- Converting EMF to PDF without cropping
- Cropping raster images with Aspose.Imaging
- Working with vector graphics and rasterization options
