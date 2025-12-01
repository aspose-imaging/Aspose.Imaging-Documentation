---
title: Convert DJVU to PDF
linktitle: Convert DJVU to PDF
type: docs
weight: 30
url: /net/convert-djvu-to-pdf/
description: Converts a DJVU document to a multi‑page PDF using Aspose.Imaging for .NET.
keywords: djvu pdf c#
---

# Convert DJVU to PDF

## Introduction
This example demonstrates how to load a DJVU image and export selected pages as a multi‑page PDF document. Use it when you need to transform DJVU files into PDF format while controlling which pages are included.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample DJVU file (e.g., `Sample.djvu`) placed in the data directory used by the example

## Step-by-step Guide
1. **Locate the data directory** – Obtain the path to the folder containing the source DJVU file.  
2. **Load the DJVU image** – Use `Image.Load` to create a `DjvuImage` instance.  
3. **Create PDF export options** – Instantiate `PdfOptions` and assign a new `PdfDocumentInfo` for metadata.  
4. **Define the page range** – Create an `IntRange` specifying the first and last pages to export (e.g., pages 0‑5).  
5. **Configure multi‑page options** – Set `PdfOptions.MultiPageOptions` with a `DjvuMultiPageOptions` object containing the defined range.  
6. **Save as PDF** – Call `image.Save` with the target PDF filename and the configured `PdfOptions`.  

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "8cb4d54ade9d8cceaa0f3bba804db38d" "ConvertDjVuToPDF.cs" >}}

## See Also
- [Convert PDF to DJVU](#)  
- [Extract images from a DJVU file](#)  
- [Batch convert multiple DJVU files to PDF](#)
