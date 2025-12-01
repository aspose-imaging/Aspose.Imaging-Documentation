---
title: Adjust Brightness in DICOM Images
linktitle: Adjust Brightness DICOM
type: docs
weight: 30
url: /net/adjust-brightness-dicom/
description: Demonstrates how to adjust the brightness of a DICOM image and save it as BMP using Aspose.Imaging for .NET.
keywords: dicom brightness c#
---

# Adjust Brightness in DICOM Images

## Introduction
This example shows how to modify the brightness of a DICOM image using Aspose.Imaging for .NET. It is useful when you need to enhance the visual appearance of medical images before further analysis or conversion.

## Prerequisites
- .NET 9.0 (or compatible version)
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data directory

## Step-by-step Guide
1. **Locate the DICOM file** – Retrieve the path to the source DICOM file.
2. **Load the image** – Use `DicomImage` to open the file stream.
3. **Adjust brightness** – Call `image.AdjustBrightness(50)` (value range: -100 to 100).
4. **Save the result** – Save the modified image as BMP using `BmpOptions`.

## Code Example
Below is the complete code for the example:

{{< gist "aspose-imaging-gists" "980862855f978a888703f8fa18ac65dc" "AdjustBrightnessDICOM.cs" >}}

## See Also
- [Convert DICOM to PNG](#)  
- [Apply Contrast to DICOM Images](#)  
- [Working with Image Metadata in Aspose.Imaging](#)
