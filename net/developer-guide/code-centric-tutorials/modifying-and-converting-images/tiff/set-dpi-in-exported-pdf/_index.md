---
title: Set DPI in Exported PDF
linktitle: Set DPI in Exported PDF
type: docs
weight: 30
url: /net/set-dpi-in-exported-pdf/
description: Demonstrates how to preserve DPI when exporting a TIFF image to PDF using Aspose.Imaging for .NET.
keywords: tiff pdf dpi c#
---

# Set DPI in Exported PDF

## Introduction
This example shows how to retain the original DPI of a TIFF image when converting it to a PDF document. Use it when you need the PDF output to match the source image's resolution for printing or high‑quality display.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library
- A sample TIFF file (e.g., `AFREY-Original.tif`) placed in the data directory used by the examples

## Step-by-step Guide
1. Load the source TIFF image using `Image.Load`.
2. Retrieve the image’s horizontal and vertical resolutions.
3. Create a `PdfOptions` instance and assign a `ResolutionSetting` with the retrieved DPI values.
4. Save the image as a PDF using the configured `PdfOptions`.
5. Optionally delete the generated PDF to clean up after verification.

## Code Example
The following code demonstrates the process:

{{< gist "aspose-imaging-gists" "36bb6c6492e7e7f3e691162cd0c1f76b" "SetDPIInExportedPdf.cs" >}}

## See Also
- **Export TIFF to JPEG** – converting TIFF images to JPEG format while preserving quality.  
- **Changing Image DPI** – adjusting DPI of various image formats before saving.  
- **Working with PDF Options** – detailed guide on customizing PDF output using Aspose.Imaging.
