---
title: Convert CDR Multipage to PSD with Merged Layers
linktitle: CDR to PSD (Multipage)
type: docs
weight: 30
url: /net/cdr-to-psd-multipage/
description: Demonstrates converting a multipage CDR file to a PSD file with merged layers using Aspose.Imaging for .NET.
keywords: cdr psd convert
---

# Convert CDR Multipage to PSD with Merged Layers

## Introduction
This example shows how to load a multipage CorelDRAW (CDR) file and export it as a single‑layer PSD file. It is useful when you need to combine all pages of a CDR document into one Photoshop layer for further editing.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A sample multipage CDR file (e.g., `MultiPage.cdr`) placed in the data directory

## Step-by-step Guide
1. **Locate the data directory** – Use the helper method `RunExamples.GetDataDir_CDR()` to obtain the folder that contains the source CDR file.  
2. **Load the CDR image** – Call `Image.Load` and cast the result to `Aspose.Imaging.FileFormats.Cdr.CdrImage`.  
3. **Create PSD export options** – Instantiate `PsdOptions` and configure `MultiPageOptions`:
   - Set `MergeLayers = true` to merge all pages into a single layer.  
4. **Configure rasterization** – Retrieve the default vector rasterization options from the CDR image and adjust text rendering and smoothing as needed.  
5. **Save the PSD file** – Call `image.Save` with the output path and the configured options.  
6. **Clean up** – Optionally delete the generated PSD file after verification.

## Code Example
The complete source code is shown below:

{{< gist "aspose-imaging-gists" "637e483a521dce5b31c458d197b312c6" "CdrToPsdMultipageExample.cs" >}}

## See Also
- Converting CDR to PNG format
- Working with multi‑page images in Aspose.Imaging
- Merging layers when exporting to PSD
