---
title: Crop DICOM Images by Shifts with Aspose.Imaging for .NET
linktitle: DICOM Cropping by Shifts
type: docs
weight: 30
url: /net/dicom-cropping-by-shifts/
description: Demonstrates cropping a DICOM image using shift values.
keywords: dicom crop c#
---

# Crop DICOM Images by Shifts

## Introduction
This example shows how to crop a DICOM image by specifying horizontal and vertical shift values. Use it when you need to trim margins or focus on a particular region of a medical image.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DICOM file named **file.dcm** placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the directory containing the DICOM file.  
2. Open the DICOM file using a `FileStream` and create a `DicomImage` instance.  
3. Call the `Crop` method on the `DicomImage` object, providing the left, top, right, and bottom shift values.  
4. Save the cropped image to a desired format (e.g., BMP) using an appropriate `ImageOptions` class.  
5. Dispose of the image and stream resources (handled automatically with `using` statements).

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b7b4d7381970eb4c8ab79f8ed9d9c64a" "DICOMCroppingByShifts.cs" >}}

## See Also
- **Converting DICOM to Other Formats** – Learn how to convert DICOM images to PNG, JPEG, and more.  
- **Applying Image Filters to DICOM** – Explore applying filters such as windowing and leveling on DICOM images.
