---
title: Flip a DICOM Image Using Aspose.Imaging for .NET
linktitle: Flip DICOM Image
type: docs
weight: 30
url: /net/flip-dicom-image/
description: Demonstrates how to flip a DICOM image and save it as BMP using Aspose.Imaging for .NET.
keywords: flip dicom c#
---

# Flip a DICOM Image Using Aspose.Imaging for .NET

## Introduction
This example shows how to open a DICOM file, apply a 180‑degree rotation (flip), and save the result as a BMP image. Use it when you need to re‑orient medical images programmatically.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data directory

## Step-by-step Guide
1. **Get the data directory** – Retrieve the path where the sample DICOM file resides.  
2. **Open the DICOM file** – Create a `FileStream` and instantiate a `DicomImage` object.  
3. **Apply rotation/flip** – Call `RotateFlip(RotateFlipType.Rotate180FlipNone)` on the image.  
4. **Save the output** – Use `BmpOptions` to save the transformed image as `FlipDICOMImage_out.bmp`.  
5. **Dispose resources** – Wrap the stream and image in `using` statements to ensure proper cleanup.

## Code Example
The following snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "b4f5386a4786cf827a164e6ece94f116" "FlipDICOMImage.cs" >}}

## See Also
- **Convert DICOM to JPEG** – Learn how to convert DICOM files to common image formats.  
- **Rotate DICOM Images** – Explore other rotation options available for DICOM images.  
- **Working with BMP Options** – Customize BMP output settings such as compression and resolution.
