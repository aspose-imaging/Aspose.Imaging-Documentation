---
title: Resize DICOM Images Using Aspose.Imaging for .NET
linktitle: DICOM Simple Resizing
type: docs
weight: 30
url: /net/dicom-simple-resizing/
description: Demonstrates how to resize a DICOM image and save it as BMP with Aspose.Imaging for .NET.
keywords: dicom resize c#
---

# Resize DICOM Images Using Aspose.Imaging for .NET

## Introduction
This example shows how to load a DICOM image, change its dimensions, and save the result in BMP format using Aspose.Imaging for .NET. It is useful when you need to preprocess medical images for display or analysis at a different resolution.

## Prerequisites
- .NET 9.0 (or later) runtime installed.
- Aspose.Imaging for .NET library referenced in the project.
- A sample DICOM file (`file.dcm`) placed in the example data directory.

## Step-by-step Guide
1. **Obtain the data directory** – Use the provided helper to locate the folder containing the DICOM sample file.  
2. **Open the DICOM file** – Create a `FileStream` for the file and instantiate a `DicomImage` object.  
3. **Resize the image** – Call `Resize(width, height)` on the `DicomImage` instance (e.g., 200 × 200 pixels).  
4. **Save the resized image** – Use `Save` with a `BmpOptions` instance to write the output as a BMP file.  
5. **Dispose resources** – The `using` statements automatically release the file stream and image resources.

## Code Example
The complete source code for this example is shown below:

{{< gist "aspose-imaging-gists" "8c48e4b5261ced4318f41dcd49cb16b5" "DICOMSimpleResizing.cs" >}}

## See Also
- Converting DICOM images to other formats.  
- Resizing images of other formats (JPEG, PNG, etc.) with Aspose.Imaging.  
- Accessing and modifying pixel data in Aspose.Imaging.
