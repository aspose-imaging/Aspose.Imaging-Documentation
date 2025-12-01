---
title: Support of DPI Settings in PDF Options
linktitle: DPI Settings in PDF
type: docs
weight: 30
url: /net/support-of-dpi-settings-in-pdf-options/
description: Demonstrates how to set DPI‑related page size when saving an image as PDF using Aspose.Imaging for .NET.
keywords: pdf dpi c#
---

# Support of DPI Settings in PDF Options

## Introduction
This example shows how to configure DPI‑related settings when converting an image to PDF. It is useful when you need to control the physical size of the resulting PDF page, such as matching specific printing dimensions.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample TIFF image file (e.g., `SampleTiff1.tiff`) placed in the example data folder

## Step-by-step Guide
1. Locate the input TIFF image using `RunExamples.GetDataDir_ModifyingAndConvertingImages()`.
2. Load the image with `Image.Load`.
3. Create a `PdfOptions` instance and set the `PageSize` property to the desired dimensions (width and height in points, where 1 point = 1/72 inch).
4. Save the image as PDF using `image.Save(outputFilePath, pdfOptions)`.
5. Verify that the generated PDF respects the specified page size.

## Code Example
Below is the complete code for this scenario:

{{< gist "aspose-imaging-gists" "53f40a5d29b3caf7380f0ca23e11e900" "SupportOfDPISettingsInPdfOptions.cs" >}}

## See Also
- Converting TIFF images to PDF with Aspose.Imaging
- Setting image resolution (DPI) when saving raster formats
- Working with PDF options in Aspose.Imaging for .NET
