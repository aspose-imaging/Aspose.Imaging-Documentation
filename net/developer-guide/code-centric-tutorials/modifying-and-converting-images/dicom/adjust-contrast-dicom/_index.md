---
title: Adjust Contrast of DICOM Images
linktitle: Adjust Contrast DICOM
type: docs
weight: 30
url: /net/adjust-contrast-dicom/
description: Demonstrates how to adjust the contrast of a DICOM image using Aspose.Imaging for .NET.
keywords: dicom contrast c#
---

# Adjust Contrast of DICOM Images

## Introduction
This example shows how to change the contrast of a DICOM image programmatically. It is useful when you need to enhance medical images for better visual analysis or preprocessing before further processing.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A DICOM file (e.g., `file.dcm`) placed in the example data directory

## Step-by-step Guide
1. **Locate the data folder** – Use the helper method `RunExamples.GetDataDir_DICOM()` to obtain the path where the source DICOM file resides.  
2. **Open the DICOM file** – Create a `FileStream` for the `.dcm` file and instantiate a `DicomImage` object from that stream.  
3. **Adjust the contrast** – Call `image.AdjustContrast(50)` (the value can be changed to increase or decrease contrast).  
4. **Save the result** – Save the modified image to a BMP file using `BmpOptions`.  

## Code Example
The following code demonstrates adjusting the contrast of a DICOM image and saving the result.

{{< gist "aspose-imaging-gists" "82cc2c46c266215d03451d81840d2d43" "AdjustContrastDICOM.cs" >}}

## See Also
- Loading and saving DICOM images with Aspose.Imaging
- Converting DICOM images to other formats
- Adjusting brightness of a DICOM image
