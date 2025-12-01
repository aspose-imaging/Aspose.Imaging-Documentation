---
title: Save EMF to File
linktitle: Save EMF to File
type: docs
weight: 30
url: /net/save-emf-to-file/
description: Demonstrates how to save an EMF image to a file using Aspose.Imaging for .NET.
keywords: EMF, save, C#
---

# Save EMF Image to File

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image and save it back to a file using Aspose.Imaging for .NET. It is useful when you need to manipulate or re‑export vector graphics stored in EMF format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An EMF file (e.g., `TestEmfBezier.emf`) placed in the example data folder

## Step-by-step Guide
1. Determine the directory that contains the source EMF file.  
2. Load the EMF file into a `MetaImage` object using `Image.Load`.  
3. Call the `Save` method on the `MetaImage` instance, providing the target file path and an `EmfOptions` object.  
4. Verify that the new file (original name with `.emf` extension) has been created.

## Code Example
Below is the complete C# code for this scenario.

{{< gist "aspose-imaging-gists" "9f55b62a9ffca1717bfe8301a2c3df9a" "SaveEMFtoFile.cs" >}}

## See Also
- Converting EMF to other raster formats
- Editing vector graphics with Aspose.Imaging
- Working with other meta file types (WMF, SVG)
