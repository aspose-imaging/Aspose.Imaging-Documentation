---
title: Convert CMX to PDF with Aspose.Imaging for .NET
linktitle: CMX to PDF
type: docs
weight: 30
url: /net/cmx-to-pdf/
description: Demonstrates converting a multi‑page CMX file to PDF using Aspose.Imaging for .NET.
keywords: cmx pdf conversion
---

# Convert CMX to PDF with Aspose.Imaging for .NET

## Introduction
This example shows how to load a CMX (CorelDRAW) file, apply rasterization settings, and save it as a PDF document. Use it when you need to programmatically convert CMX artwork to PDF while preserving vector quality.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample CMX file (e.g., `MultiPage.cmx`) placed in the example’s data directory

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path where the example CMX file resides.  
2. **Load the CMX image** – Use `Image.Load` to open the CMX file as a `CmxImage`.  
3. **Create PDF options** – Instantiate `PdfOptions` and set up a `PdfDocumentInfo` object.  
4. **Configure rasterization** – Obtain default rasterization options from the CMX image and adjust text rendering and smoothing settings as needed.  
5. **Save as PDF** – Call `image.Save` with the target PDF file name and the configured `PdfOptions`.  
6. **Clean up** – Optionally delete the generated PDF to keep the demo output tidy.

## Code Example
The following code demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "cae9716d6ceebbd2322cfacdddc88472" "CmxToPdfExample.cs" >}}

## See Also
- Converting SVG to PDF with Aspose.Imaging  
- Rasterizing vector images to PNG in .NET  
- Working with PDF documents using Aspose.Imaging for .NET
