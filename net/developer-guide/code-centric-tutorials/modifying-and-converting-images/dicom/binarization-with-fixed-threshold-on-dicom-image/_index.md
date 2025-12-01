---
title: Binarize a DICOM Image Using a Fixed Threshold
linktitle: Fixed Threshold Binarization
type: docs
weight: 30
url: /net/binarization-with-fixed-threshold-on-dicom-image/
description: Demonstrates how to binarize a DICOM image with a fixed threshold using Aspose.Imaging for .NET.
keywords: dicom binarize c#
---

# Binarize a DICOM Image Using a Fixed Threshold

## Introduction
This example shows how to convert a DICOM medical image to a binary (black‑and‑white) image by applying a predefined fixed threshold. Use it when you need to highlight structures in radiology images or prepare data for further analysis.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DICOM file (`file.dcm`) placed in the example data directory

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path that contains the source DICOM file.  
2. **Open the DICOM image** – Use `DicomImage` to load the image from a file stream.  
3. **Apply fixed‑threshold binarization** – Call `BinarizeFixed` with the desired threshold value (e.g., `100`).  
4. **Save the result** – Export the binarized image to a BMP file (or any supported format) using `BmpOptions`.  

## Code Example
The following code shows the complete example:

{{< gist "aspose-imaging-gists" "071abcfae837036d095338769eeb8b93" "BinarizationWithFixedThresholdOnDICOMImage.cs" >}}

## See Also
- Converting DICOM images to other formats  
- Applying other image filters with Aspose.Imaging  
- Working with medical images in Aspose.Imaging for .NET
