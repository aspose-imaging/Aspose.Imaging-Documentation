---
title: Convert EMF to WMF Using Aspose.Imaging for .NET
linktitle: Convert EMF to WMF
type: docs
weight: 30
url: /net/convert-emf-to-wmf/
---

# Convert EMF to WMF

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image and save it as a WMF (Windows Metafile) using Aspose.Imaging for .NET. It is useful when you need to work with vector graphics and require WMF output for compatibility with legacy applications.

## Prerequisites
- .NET 9.0 or later
- Aspose.Imaging for .NET library
- Sample EMF file (e.g., `Picture1.emf`) placed in the data directory used by the example

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder that contains the source EMF file.
2. **Load the EMF image** – Use `Image.Load` to read the EMF file into an `Image` object.
3. **Configure rasterization options** – Access the default options, cast the vector rasterization options to `EmfRasterizationOptions`, and adjust properties such as background color, page size, and borders.
4. **Save as WMF** – Call `image.Save` with the same options, specifying a `.wmf` file name for the output.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "d0acedb06fa0c40dc7da996a1292d818" "ConvertEMFToWMF.cs" >}}

## See Also
- Converting PNG to JPEG with Aspose.Imaging for .NET
- Modifying vector images (e.g., scaling, rotating) using Aspose.Imaging
- Rasterizing EMF files to bitmap formats
