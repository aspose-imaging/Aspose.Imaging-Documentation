---
title: Remove Metadata from DICOM Image and Save with Metadata
linktitle: Remove Metadata (DICOM)
type: docs
weight: 30
url: /net/remove-metadata/
description: Demonstrates how to remove or retain metadata when saving DICOM images using Aspose.Imaging for .NET.
keywords: dicom metadata c#
---

# Remove Metadata from DICOM Image and Save with Metadata

## Introduction
This example shows how to work with metadata in DICOM images using Aspose.Imaging for .NET. It covers removing metadata, keeping metadata during export, and modifying metadata before saving. Use it when you need fine‑grained control over DICOM file information.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DICOM file (`file.dcm`) placed in the example data directory

## Step-by-step Guide
1. Load the source DICOM image with `Image.Load`.
2. Choose an export option:
   - Set `KeepMetadata = true` to retain metadata.
   - Call `RemoveMetadata()` on the image to strip all metadata.
3. (Optional) Modify EXIF data, e.g., update the `UserComment` field.
4. Save the image to the desired output path using the configured options.
5. Clean up any temporary files created during the process.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "99b42e4cbf68213eb511e5d0be0e6fa8" "RemoveAndSaveWithMetadata.cs" >}}

## See Also
- Export DICOM with metadata preserved
- Modify EXIF data in images
- Working with DICOM images using Aspose.Imaging for .NET
