---
title: Convert a Range of DjVu Pages to Multi-Page TIFF
linktitle: Convert Range of DjVu Pages
type: docs
weight: 20
url: /net/convert-range-of-djvu-pages/
description: Demonstrates how to export a specific range of pages from a DjVu document to a multi‑page TIFF file using Aspose.Imaging for .NET.
keywords: djvu, tiff, c#
---

# Convert a Range of DjVu Pages to Multi‑Page TIFF

## Introduction
This example shows how to load a DjVu document, select a specific range of pages, and export those pages as a multi‑page TIFF file. Use it when you need to extract and convert only part of a DjVu document rather than processing the entire file.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A DjVu sample file named `Sample.djvu` placed in the data directory

## Step-by-step Guide
1. **Initialize the data directory** – Obtain the path where the sample DjVu file resides.  
2. **Load the DjVu image** – Use `Image.Load` to open the DjVu document.  
3. **Create TIFF export options** – Instantiate `TiffOptions` with the desired compression format.  
4. **Define the page range** – Create an `IntRange` specifying the start and end page indices you want to export.  
5. **Configure multi‑page options** – Assign a `DjvuMultiPageOptions` object (initialized with the `IntRange`) to the `MultiPageOptions` property of the `TiffOptions`.  
6. **Save the result** – Call `image.Save` with a target file name and the configured `TiffOptions` to generate the multi‑page TIFF file.

## Code Example
The following snippet contains the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "cec93d0d381642fe9f74340f6f8bbc1b" "ConvertRangeOfDjVuPages.cs" >}}

## See Also
- [Convert DjVu to PDF](../convert-djvu-to-pdf/)
- [Extract Individual Pages from a DjVu Document](../extract-djvu-pages/)
- [Create Multi-Page TIFF from Multiple Images](../create-multipage-tiff/)
