---
title: Converting EMF to WMF Using Aspose.Imaging for .NET
linktitle: Convert EMF to WMF
type: docs
weight: 30
url: /net/converting-emf-to-wmf/
description: Demonstrates how to convert EMF images to WMF format with Aspose.Imaging for .NET.
keywords: emf wmf conversion c#
---

# Convert EMF Images to WMF Format

## Introduction
This example shows how to load EMF (Enhanced Metafile) images and convert them to WMF (Windows Metafile) format using Aspose.Imaging for .NET. Use it when you need to change metafile types for compatibility with older Windows applications.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample EMF files (e.g., `TestEmfRotatedText.emf`, `TestEmfPlusFigures.emf`, `TestEmfBezier.emf`)

## Step-by-step Guide
1. Prepare the folder path that contains the source EMF files.  
2. Create an array with the names of the EMF files to be processed.  
3. Iterate over each file name:
   - Combine the folder path and file name to obtain the full file path.  
   - Load the EMF image using `Image.Load` and cast it to `MetaImage`.  
   - Save the image as WMF by calling `MetaImage.Save` with a `WmfOptions` instance and appending `_out.wmf` to the original file name.

## Code Example
Below is the complete code snippet for this conversion task:

{{< gist "aspose-imaging-gists" "7b697ba636f0c8b0643930eb45417b5e" "ConvertingEMFToWMF.cs" >}}

## See Also
- Converting PNG to JPEG with Aspose.Imaging for .NET  
- Adding watermarks to images using Aspose.Imaging  
- Working with vector graphics in Aspose.Imaging
