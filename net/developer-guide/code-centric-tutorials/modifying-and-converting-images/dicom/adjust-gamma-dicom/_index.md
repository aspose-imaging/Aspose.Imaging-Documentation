---
title: Adjust Gamma in DICOM Images using Aspose.Imaging for .NET
linktitle: Adjust Gamma DICOM
type: docs
weight: 30
url: /net/adjust-gamma-dicom/
description: Demonstrates how to adjust the gamma of a DICOM image and save the result as a BMP file.
keywords: dicom,gamma,c#
---

# Adjust Gamma in DICOM Images

## Introduction
This example shows how to modify the gamma level of a DICOM image using Aspose.Imaging for .NET. Adjusting gamma can improve the visual clarity of medical images, making them easier to analyze. Use this guide when you need to enhance DICOM images before further processing or display.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data folder

## Step-by-step Guide
1. **Locate the data directory** – Obtain the path to the folder containing the DICOM file.
2. **Open the DICOM file** – Create a `FileStream` for `file.dcm` and initialize a `DicomImage` instance.
3. **Adjust gamma** – Call `AdjustGamma` on the `DicomImage` object with the desired gamma value (e.g., 50).
4. **Save the result** – Use `BmpOptions` to specify BMP format and save the processed image as `AdjustGammaDICOM_out.bmp`.
5. **Dispose resources** – Ensure all streams and image objects are properly closed after the operation.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "65ea7da6ed4ae23c4750a05d4a44eaef" "AdjustGammaDICOM.cs" >}}

## See Also
- Converting DICOM images to other formats
- Adjusting brightness and contrast of images
- Working with BMP options in Aspose.Imaging for .NET
