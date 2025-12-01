---
title: Support DICOM YBR422 Color Space Conversion
linktitle: Support DICOM YBR422
type: docs
weight: 30
url: /net/support-dicom-ybr422/
description: Demonstrates how to load a DICOM image and save it as PNG using Aspose.Imaging for .NET.
keywords: dicom c# aspose-imaging
---

# Support DICOM YBR422 Color Space Conversion

## Introduction
This example shows how to work with DICOM images that use the YBR422 colour space. It loads a DICOM file, converts it to a PNG image, and then cleans up the generated file. Use this when you need to process medical images and convert them to a more common format for further analysis or display.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DICOM file named `input.dcm` placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the DICOM data directory using the provided helper method.  
2. Combine the directory path with the file name `input.dcm` to create the full input path.  
3. Load the DICOM image with `Image.Load`.  
4. Save the loaded image as a PNG file by appending `.png` to the original path.  
5. Delete the temporary PNG file to clean up after the conversion.  

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "a6613e94bee77421fb5f30c90e861bb2" "SupportDicomYBR422.cs" >}}

## See Also
- Converting DICOM to Other Formats
- Working with Image Formats in Aspose.Imaging
- Loading and Saving Images with Aspose.Imaging for .NET
