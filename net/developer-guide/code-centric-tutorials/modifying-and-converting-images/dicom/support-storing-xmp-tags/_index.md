---
title: Support Storing XMP Tags in DICOM Images
linktitle: Support Storing XMP Tags
type: docs
weight: 30
url: /net/support-storing-xmp-tags/
description: Demonstrates how to store XMP metadata tags in a DICOM image using Aspose.Imaging for .NET.
keywords: dicom, xmp, c#
---

# Support Storing XMP Tags in DICOM Images

## Introduction
This example shows how to embed XMP metadata into a DICOM image file. It is useful when you need to add detailed patient, equipment, or study information that complies with DICOM standards while preserving the image data.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- A DICOM file (`file.dcm`) placed in the example data folder

## Step-by-step Guide
1. Load the source DICOM image using `Image.Load`.
2. Create an `XmpPacketWrapper` and a `DicomPackage` to hold XMP tags.
3. Populate the `DicomPackage` with desired metadata (e.g., patient name, institution, study description).
4. Add the package to the XMP wrapper and save the image with `DicomOptions` that includes the XMP data.
5. (Optional) Reload the saved image to verify that the XMP tags were added correctly.
6. Clean up any temporary files created during the process.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "167d2d07047126af30a058bbe4b20e3b" "SupportStoringXmpTags.cs" >}}

## See Also
- Adding XMP metadata to JPEG images
- Converting DICOM images to other formats with Aspose.Imaging
- Reading and modifying DICOM tags in .NET
