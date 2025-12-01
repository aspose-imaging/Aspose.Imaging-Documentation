---
title: Crop EMF Image by Rectangle and Save as PDF
linktitle: Crop EMF Image
type: docs
weight: 30
url: /net/cropping-by-rectangle-emf-image/
description: Demonstrates how to crop an EMF image using a rectangle and export it to PDF.
keywords: emf crop pdf c#
---

# Crop EMF Image by Rectangle and Save as PDF

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image, crop it to a specified rectangular area, and save the result as a PDF document. Use it when you need to extract a portion of a vector image and convert it to a rasterized PDF.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- An EMF file named `Picture1.emf` placed in the example data directory

## Step-by-step Guide
1. **Set up rasterization options** – Configure `EmfRasterizationOptions` (e.g., background color).
2. **Create PDF options** – Assign the rasterization options to a `PdfOptions` instance.
3. **Load the EMF image** – Use `Image.Load` to read the EMF file.
4. **Crop the image** – Call `image.Crop` with a `Rectangle` that defines the desired area.
5. **Adjust page dimensions** – Set `PageWidth` and `PageHeight` on the rasterization options to match the cropped image size.
6. **Save to PDF** – Use `image.Save` with the PDF options to write the output file.

## Code Example
The following code demonstrates the process described above:

{{< gist "aspose-imaging-gists" "272127e44ac3c63fe428fa0d25ceb2a1" "CroppingByRectangleEMFImage.cs" >}}

## See Also
- **Converting EMF to PNG** – Learn how to rasterize an EMF image directly to a PNG file.  
- **Manipulating Vector Images** – Explore other operations such as scaling and rotating vector graphics.  
- **Advanced PDF Options** – Customize PDF output settings like compression and security.
