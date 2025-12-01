---
title: Convert DICOM to PNG using Aspose.Imaging for .NET
linktitle: DICOM to PNG
type: docs
weight: 30
url: /net/dicom-to-png/
description: Demonstrates how to convert a DICOM image to PNG format.
keywords: dicom png c#
---

# Convert DICOM to PNG using Aspose.Imaging for .NET

## Introduction
This example shows how to load a DICOM image and save it as a PNG file using Aspose.Imaging for .NET. It is useful when you need to work with medical imaging data and export it to a more widely supported image format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DICOM file (e.g., `MultiframePage1.dicom`) placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the directory that contains the DICOM sample file.  
2. Load the DICOM image using `Image.Load` and cast it to `DicomImage`.  
3. Create a `PngOptions` instance to configure PNG output settings.  
4. Call `Save` on the DICOM image instance, specifying the output file name and the PNG options.  
5. (Optional) Delete the generated PNG file if you only need to demonstrate the conversion process.

## Code Example
Below is the complete example code that performs the conversion:

{{< gist "aspose-imaging-gists" "d7de039e68252d63ce21c6c2e4fb83c1" "DicomToPngExample.cs" >}}

## See Also
- Converting DICOM to JPEG
- Working with multi‑frame DICOM images
- Exporting medical images to BMP format
