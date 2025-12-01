---
title: Grayscaling a DICOM Image Using Aspose.Imaging for .NET
linktitle: Grayscale DICOM Image
type: docs
weight: 30
url: /net/grayscaling-on-dicom/
description: Demonstrates how to convert a DICOM image to grayscale and save it as BMP using Aspose.Imaging for .NET.
keywords: dicom grayscale c#
---

# Grayscale a DICOM Image with Aspose.Imaging for .NET

## Introduction
This example shows how to load a DICOM file, transform it to its grayscale representation, and save the result as a BMP image. Use it when you need to simplify medical images for analysis or visualization.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DICOM file (`file.dcm`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the folder containing the DICOM file.
2. Open the DICOM file using a `FileStream`.
3. Create a `DicomImage` instance from the stream.
4. Call the `Grayscale()` method to convert the image.
5. Save the resulting image in BMP format using `BmpOptions`.

## Code Example
Below is the complete code for this scenario.

{{< gist "aspose-imaging-gists" "3ebff0a0c6f60b0fbd855d7e3cd7eedd" "GrayscalingOnDICOM.cs" >}}

## See Also
- Converting DICOM to other formats
- Applying window/level adjustments to DICOM images
- Working with medical image metadata in Aspose.Imaging for .NET
