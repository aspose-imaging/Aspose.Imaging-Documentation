---
title: Convert DjVu to TIFF
linktitle: Convert DjVu to TIFF
type: docs
weight: 30
url: /net/convert-djvu-to-tiff/
description: Convert a DjVu image to a multi‑page TIFF using Aspose.Imaging for .NET.
keywords: djvu tiff conversion
---

# Convert DjVu to TIFF

## Introduction
This example demonstrates how to load a DjVu file and save it as a multi‑page TIFF image. Use it when you need to transform DjVu documents into a widely supported TIFF format for archival or further processing.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Sample DjVu file (`Sample.djvu`) placed in the example data directory

## Step-by-step Guide
1. **Set up the data directory** – Retrieve the path where the sample DjVu file resides.  
2. **Load the DjVu image** – Use `Image.Load` to open the DjVu file as a `DjvuImage` object.  
3. **Configure TIFF options** – Create a `TiffOptions` instance with the desired compression (e.g., `TiffDeflateBw`).  
4. **Enable multi‑page support** – Assign a `DjvuMultiPageOptions` object to the `MultiPageOptions` property of the TIFF options.  
5. **Save the image** – Call `image.Save` with the target TIFF file name and the configured options.  

## Code Example
The following code demonstrates how to perform the conversion:

{{< gist "aspose-imaging-gists" "8ef8a04a67af476785b615d50ef49f88" "ConvertDjVuToTIFF.cs" >}}

## See Also
- Converting DjVu to PDF
- Working with multi‑page TIFF images
- Aspose.Imaging image loading and saving options
