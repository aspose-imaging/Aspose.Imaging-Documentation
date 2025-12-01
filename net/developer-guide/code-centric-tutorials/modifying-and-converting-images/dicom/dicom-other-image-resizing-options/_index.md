---
title: Resize DICOM Images with Different Options using Aspose.Imaging for .NET
linktitle: DICOM Image Resizing Options
type: docs
weight: 30
url: /net/dicom-other-image-resizing-options/
description: Demonstrates how to resize DICOM images proportionally using different resize types.
keywords: dicom resize c#
---

# Resize DICOM Images with Different Options

## Introduction
This example shows how to resize DICOM images by adjusting height or width proportionally while preserving image quality. It uses the `ResizeHeightProportionally` and `ResizeWidthProportionally` methods with the `AdaptiveResample` resize type, which is ideal when you need precise control over medical image scaling.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A DICOM file (`file.dcm`) placed in the example data directory

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path where the DICOM source file resides.  
2. **Open the DICOM file** – Create a `FileStream` for the DICOM file and instantiate a `DicomImage` object using the stream.  
3. **Resize by height** – Call `ResizeHeightProportionally` with the desired height (e.g., 100 pixels) and specify `ResizeType.AdaptiveResample`.  
4. **Save the resized image** – Use `BmpOptions` (or another format) to save the output file (e.g., `DICOMSOtherImageResizingOptions_out.bmp`).  
5. **Resize by width** – Repeat steps 2‑4, this time calling `ResizeWidthProportionally` with a target width (e.g., 150 pixels).  
6. **Verify the output** – The two BMP files demonstrate how the original DICOM image has been resized using different dimensions.

## Code Example
The following snippet contains the complete working code for this scenario:

{{< gist "aspose-imaging-gists" "42d6676c6d816e876228600bdcced33e" "DICOMSOtherImageResizingOptions.cs" >}}

## See Also
- Converting DICOM images to other formats
- Adjusting DICOM image contrast and brightness
- Extracting and modifying DICOM metadata with Aspose.Imaging
