---
title: Apply Filter on DICOM Image
linktitle: Apply Filter (DICOM)
type: docs
weight: 10
url: /net/apply-filter-on-dicom-image/
description: Demonstrates how to apply a median filter to a DICOM image and save the result.
keywords: dicom filter c#
---

# Apply Filter on DICOM Image

## Introduction
This example shows how to apply a median filter to a DICOM image using Aspose.Imaging for .NET. Filtering can enhance image quality by reducing noise, which is useful in medical imaging workflows. After filtering, the image is saved in BMP format for further processing or visualization.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data directory

## Step-by-step Guide
1. **Set up the data directory** – Retrieve the path where the DICOM file is stored.  
2. **Open the DICOM file** – Use `FileStream` to read the file and create a `DicomImage` instance.  
3. **Apply the median filter** – Call the `Filter` method with `MedianFilterOptions` (kernel size 8) over the image bounds.  
4. **Save the filtered image** – Export the result to BMP format using `BmpOptions`.  
5. **Dispose resources** – The `using` statements ensure that both the file stream and the image are properly released.

## Code Example
The following snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "93ded5be73c17bdba2041be62e4db276" "ApplyFilterOnDICOMImage.cs" >}}

## See Also
- Converting DICOM images to other formats
- Applying different image filters with Aspose.Imaging
- Working with DICOM metadata in Aspose.Imaging for .NET
