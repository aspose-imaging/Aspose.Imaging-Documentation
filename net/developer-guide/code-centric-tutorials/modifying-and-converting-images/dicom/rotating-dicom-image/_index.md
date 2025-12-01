---
title: Rotating a DICOM Image Using Aspose.Imaging for .NET
linktitle: Rotate DICOM Image
type: docs
weight: 30
url: /net/rotating-dicom-image/
description: Demonstrates how to rotate a DICOM image and save it as BMP with Aspose.Imaging for .NET.
keywords: dicom rotate c#
---

# Rotating a DICOM Image

## Introduction
This example shows how to rotate a DICOM image by a specified angle and then save the transformed image in BMP format. It is useful when you need to adjust the orientation of medical images before further processing or display.

## Prerequisites
- .NET 9.0 (or later) development environment
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data directory

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the folder that contains the source DICOM file.
2. **Open the DICOM file** – Create a `FileStream` for the `file.dcm` using read access.
3. **Load the image** – Instantiate a `DicomImage` from the file stream.
4. **Apply rotation** – Call the `Rotate` method with the desired angle (e.g., 10 degrees).
5. **Save the result** – Export the rotated image to BMP format using `BmpOptions`.
6. **Dispose resources** – Ensure all streams and image objects are properly closed.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "8d338d601c4646a92334a18c9fa806af" "RotatingDICOMImage.cs" >}}

## See Also
- **Converting DICOM to other formats** – Learn how to convert DICOM images to JPEG, PNG, or TIFF.
- **Applying other transformations** – Explore scaling, cropping, and flipping operations on images.
- **Working with DICOM metadata** – Access and modify DICOM tags using Aspose.Imaging.
