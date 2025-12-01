---
title: Dithering a DICOM Image
linktitle: Dithering DICOM Image
type: docs
weight: 30
url: /net/dithering-for-dicom-image/
description: Demonstrates how to apply threshold dithering to a DICOM image using Aspose.Imaging for .NET.
keywords: dithering dicom c#
---

# Dithering a DICOM Image

## Introduction
This example shows how to apply threshold dithering to a DICOM image and save the processed image as a BMP file. Use it when you need to reduce image complexity while preserving essential visual information in medical imaging workflows.

## Prerequisites
- .NET 6.0 or later (compatible with your project)
- Aspose.Imaging for .NET library
- A DICOM file (e.g., `file.dcm`) placed in the data directory used by the example

## Step-by-step Guide
1. Determine the path to the folder containing the source DICOM file.  
2. Open the DICOM file using `DicomImage`.  
3. Call the `Dither` method with `DitheringMethod.ThresholdDithering` and an appropriate threshold value (e.g., `1`).  
4. Save the resulting image in the desired format (BMP in this case) using `BmpOptions`.  

## Code Example
The following code demonstrates how to perform threshold dithering on a DICOM image and save the result:

{{< gist "aspose-imaging-gists" "9934c2bbfa3005572f16f9abecbd96ff" "DitheringForDICOMImage.cs" >}}

## See Also
- Converting DICOM images to other formats  
- Applying other dithering methods (e.g., Floyd‑Steinberg) with Aspose.Imaging  
- General image processing techniques in the Aspose.Imaging for .NET library
