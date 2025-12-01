---
title: Create Indexed PSD Files
linktitle: Indexed PSD Files
type: docs
weight: 30
url: /net/create-indexed-psd-files/
description: Demonstrates how to create an indexed PSD file with a custom color palette using Aspose.Imaging for .NET.
keywords: psd, indexed, create
---

# Create Indexed PSD Files

## Introduction
This example shows how to generate a new PSD file with an indexed color palette and RLE compression. Use it when you need to programmatically create PSD files with a limited set of colors, such as for thumbnails or specialized graphics workflows.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Access to a writable folder for output files (the example writes `CreateIndexedPSDFiles_out.psd`)

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder where the PSD will be saved.
2. **Configure `PsdOptions`** –  
   - Specify the output file path with `FileCreateSource`.  
   - Set `ColorMode` to `Rgb`.  
   - Choose the PSD version (e.g., 5).  
   - Define a small color palette (e.g., Red, Green, Blue).  
   - Assign `CompressionMethod` (RLE) for efficient storage.
3. **Create the PSD image** – Call `Image.Create` with the configured options and desired dimensions (e.g., 500×500).
4. **Draw graphics** – Use `Graphics` to clear the background and draw an ellipse or other shapes.
5. **Save the file** – Persist the image to the specified path.

## Code Example
Below is the complete code for the example:

{{< gist "aspose-imaging-gists" "c19c4eeb04dae11a5508b419e1b86965" "CreateIndexedPSDFiles.cs" >}}

## See Also
- [Working with PSD Files – Basics](../psd-basics)
- [Applying Custom Color Palettes to Images](../color-palettes)
- [Saving Images with Compression Options](../compression-methods)
