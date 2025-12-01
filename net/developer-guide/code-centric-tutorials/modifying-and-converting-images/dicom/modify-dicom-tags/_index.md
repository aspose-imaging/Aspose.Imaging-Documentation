---
title: Modify DICOM Tags with Aspose.Imaging for .NET
linktitle: Modify DICOM Tags
type: docs
weight: 30
url: /net/modify-dicom-tags/
description: Shows how to update, add, and remove DICOM tags using Aspose.Imaging for .NET.
keywords: dicom, tags, c#
---

# Modify DICOM Tags with Aspose.Imaging for .NET

## Introduction
This example demonstrates how to manipulate DICOM metadata—updating, adding, and removing tags—using the Aspose.Imaging for .NET library. It is useful when you need to edit patient information or other DICOM attributes programmatically.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DICOM file named `file.dcm` placed in the example data folder

## Step-by-step Guide
1. **Locate the data directory** – retrieve the path where the DICOM test file resides.  
2. **Load the DICOM image** – use `Image.Load` to create a `DicomImage` instance.  
3. **Update an existing tag** – call `FileInfo.UpdateTagAt` with the tag index and new value (e.g., Patient's Name).  
4. **Add a new tag** – use `FileInfo.AddTag` to insert a custom tag with its value.  
5. **Remove an unwanted tag** – invoke `FileInfo.RemoveTagAt` with the appropriate index.  
6. **Save the modified image** – call `Save` to write changes to a new DICOM file.  
7. **Clean up** – delete the temporary output file if it is no longer required.

## Code Example
The following code demonstrates the process:

{{< gist "aspose-imaging-gists" "f111aae5ca0434ec9adef570af085bff" "ModifyDicomTags.cs" >}}

## See Also
- Working with DICOM Images in Aspose.Imaging
- Converting DICOM to Other Formats
- Modifying Image Metadata with Aspose.Imaging
