---
title: Binarize a DICOM Image Using Otsu Threshold
linktitle: Binarize DICOM with Otsu
type: docs
weight: 30
url: /net/binarization-with-otsu-threshold-on-dicom-image/
description: Demonstrates how to binarize a DICOM image using Otsu thresholding with Aspose.Imaging for .NET.
keywords: dicom, binarize, otsu
---

# Binarize a DICOM Image Using Otsu Threshold

## Introduction
This example shows how to apply Otsu thresholding to a DICOM image and save the result as a bitmap. Use it when you need to convert medical images into a binary format for further analysis or display.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET
- A DICOM file named **file.dcm** placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the DICOM source file.  
2. Open the DICOM file using `DicomImage`.  
3. Call `BinarizeOtsu()` on the image to perform Otsu thresholding.  
4. Save the processed image to a bitmap file using `BmpOptions`.

## Code Example
The following code snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "816ee269909d9861564fe9716863d452" "BinarizationWithOtsuThresholdOnDICOMImage.cs" >}}

## See Also
- Converting DICOM images to other formats  
- Applying other image processing operations with Aspose.Imaging  
- Working with medical image metadata in Aspose.Imaging
