---
title: Convert OTG to PNG and PDF Using Aspose.Imaging for .NET
linktitle: Support of OTG
type: docs
weight: 30
url: /net/support-of-otg/
description: Demonstrates how to rasterize OTG files to PNG and PDF formats with Aspose.Imaging for .NET.
keywords: otg rasterization c#
---

# Convert OTG to PNG and PDF Using Aspose.Imaging for .NET

## Introduction
This example shows how to load an OTG (OpenType Glyph) file and rasterize each page into both PNG and PDF formats. Use it when you need to convert vector-based OTG documents to common image or document types.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An OTG file named **VariousObjectsMultiPage.otg** placed in the example data folder

## Step-by-step Guide
1. Obtain the path to the OTG file using the provided helper method.  
2. Create an array of rasterization options: `PngOptions` and `PdfOptions`.  
3. For each option, determine the appropriate file extension (`.png` or `.pdf`).  
4. Load the OTG image with `Image.Load`.  
5. Configure `OtgRasterizationOptions` to match the source image size.  
6. Assign the rasterization options to the current `ImageOptionsBase` instance.  
7. Save the rasterized output to the data folder using the determined extension.

## Code Example
The following code demonstrates the conversion process:

{{< gist "aspose-imaging-gists" "e0cd3053bbb7628655f76209f2c8e33a" "SupportOfOTG.cs" >}}

## See Also
- Loading and saving images with Aspose.Imaging
- Working with multi-page images
- Using vector rasterization options in Aspose.Imaging
