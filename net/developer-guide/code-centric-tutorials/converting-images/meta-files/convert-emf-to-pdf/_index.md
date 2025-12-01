---
title: Convert EMF to PDF with Aspose.Imaging for .NET
linktitle: Convert EMF to PDF
type: docs
weight: 30
url: /net/convert-emf-to-pdf/
description: Convert an EMF image to PDF using Aspose.Imaging for .NET.
keywords: emf pdf conversion c#
---

# Convert EMF to PDF

## Introduction
This example demonstrates how to load an EMF (Enhanced Metafile) image and save it as a PDF document using Aspose.Imaging for .NET. It is useful when you need to convert vector‑based EMF files to PDF while preserving their visual fidelity.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An EMF file (e.g., `Picture1.emf`) placed in the example data directory

## Step-by-step Guide
1. **Get the data directory** – Retrieve the path where the input EMF file resides.  
2. **Load the EMF image** – Use `Image.Load` to read the EMF file as an `EmfImage`.  
3. **Validate the EMF header** – Ensure the image is a valid EMF before processing.  
4. **Configure rasterization options** – Set page size and background color via `EmfRasterizationOptions`.  
5. **Create PDF options** – Assign the rasterization settings to a `PdfOptions` instance.  
6. **Save as PDF** – Call `image.Save` with an output stream and the PDF options to generate the PDF file.  
7. **Handle resources** – Use `using` statements to automatically dispose of streams and image objects.

## Code Example
The following code shows the complete implementation:

{{< gist "aspose-imaging-gists" "8f28679a188ff0330f306941e51dac44" "ConvertEMFToPDF.cs" >}}

## See Also
- Converting other metafile formats to PDF
- Rasterizing EMF images to PNG
- Using vector rasterization options with Aspose.Imaging
