---
title: Create EMF Meta File Image and Save as PDF
linktitle: Create EMF Meta File Image
type: docs
weight: 30
url: /net/create-emf-meta-file-image/
description: Creates an EMF meta‑file image using Aspose.Imaging for .NET and saves it as a PDF document.
keywords: emf pdf c#
---

# Create EMF Meta File Image and Save as PDF

## Introduction
This example demonstrates how to generate an EMF meta‑file image, draw various graphics on it, and then rasterize the result into a PDF file using Aspose.Imaging for .NET. Use it when you need vector‑based drawings that must be exported to PDF.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library installed
- No additional external files are required; the example creates all drawing elements programmatically.

## Step-by-step Guide
1. **Create an `EmfRecorderGraphics2D` canvas** with the desired size.
2. **Draw shapes** (lines, rectangles, polygons) using `Pen`, `Brush`, and other graphics objects.
3. **Configure background and line styles** as needed (e.g., line caps, line joins).
4. **Finalize the drawing** by calling `EndRecording()` to obtain an `EmfImage`.
5. **Set up `PdfOptions`** with `EmfRasterizationOptions` so the EMF is rasterized correctly.
6. **Save the EMF image as a PDF** using `image.Save(outputPath, pdfOptions)`.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "f9b0cf7de4207bdbf17fbd516c71a946" "CreateEMFMetaFileImage.cs" >}}

## See Also
- [Converting EMF to Other Formats](#)  
- [Working with Vector Graphics in Aspose.Imaging](#)  
- [Saving Images to PDF with Rasterization Options](#)
