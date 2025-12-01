---
title: Extract Pages from a Multipage DjVu Image
linktitle: Multipage Image Extraction
type: docs
weight: 30
url: /net/common-multipage-image-example/
description: Demonstrates how to extract single or multiple pages from a DjVu multipage image and save them as PNG or TIFF.
keywords: multipage image c#
---

# Extract Pages from a Multipage DjVu Image

## Introduction
This example shows how to work with multipage images using Aspose.Imaging for .NET. It extracts specific pages from a DjVu document and saves them in different formats such as PNG and TIFF. Use this when you need to process or export individual pages from a multipage source.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample DjVu file (`Sample.djvu`) placed in the data directory used by the examples

## Step-by-step Guide
1. Locate the data directory that contains the source DjVu file.  
2. Load the DjVu image using `Image.Load`.  
3. Verify that the loaded image implements `IMultipageImage` and retrieve the page count if needed.  
4. Define the page range you want to export (e.g., start page 3, count 1).  
5. Create a `PngOptions` instance and set its `MultiPageOptions` with the desired page range.  
6. Save the selected page(s) as a PNG file.  
7. Adjust the page range for multiple pages (e.g., start page 0, count 2).  
8. Create a `TiffOptions` instance (choose appropriate compression) and set its `MultiPageOptions`.  
9. Save the selected pages as a TIFF file.

## Code Example
The following snippet demonstrates the complete workflow described above:

{{< gist "aspose-imaging-gists" "cdfed1c65d611da71b06a95bc061e7f0" "CommonMultipageImageExample.cs" >}}

## See Also
- [Convert Multipage TIFF to Individual Images](#)
- [Work with DjVu Images in Aspose.Imaging](#)
- [Save Images in Different Formats with Aspose.Imaging](#)
