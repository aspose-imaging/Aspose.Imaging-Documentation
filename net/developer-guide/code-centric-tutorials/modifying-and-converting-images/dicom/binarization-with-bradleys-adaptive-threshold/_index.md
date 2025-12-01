---
title: Binarization with Bradley's Adaptive Threshold
linktitle: Binarization (Bradley)
type: docs
weight: 30
url: /net/binarization-with-bradleys-adaptive-threshold/
description: Demonstrates how to binarize a DICOM image using Bradley's adaptive threshold method.
keywords: dicom, binarize, adaptive-threshold
---

# Binarization with Bradley's Adaptive Threshold

## Introduction
This example shows how to apply Bradley's adaptive threshold to a DICOM image and save the resulting bitmap. It is useful when you need to convert grayscale medical images into binary form for further analysis or visualization.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DICOM file named `image.dcm` placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder containing the DICOM test files.  
2. Open the DICOM file using `FileStream` and create a `DicomImage` instance.  
3. Call `BinarizeBradley` on the `DicomImage` object, specifying the desired window size (e.g., `10`).  
4. Save the processed image as a BMP file using `BmpOptions`.  

## Code Example
The following code snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "c0c1dd2e0cd20d5d171a461be331388f" "BinarizationWithBradleysAdaptiveThreshold.cs" >}}

## See Also
- Converting DICOM to other image formats
- Applying different binarization techniques with Aspose.Imaging
- Working with medical image metadata in .NET
