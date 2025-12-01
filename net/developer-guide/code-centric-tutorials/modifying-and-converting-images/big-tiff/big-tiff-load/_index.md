---
title: Load and Save a BigTIFF Image with Aspose.Imaging for .NET
linktitle: Load BigTIFF
type: docs
weight: 30
url: /net/big-tiff-load/
description: Demonstrates how to load a BigTIFF image and save it using Aspose.Imaging for .NET.
keywords: big tiff c#
---

# Load and Save a BigTIFF Image

## Introduction
This example illustrates how to load a BigTIFF image, convert it to a standard TIFF format, and then save it using Aspose.Imaging for .NET. It is useful when working with very large TIFF files that require the BigTIFF extensions.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An input file named **input-BigTiff.tif** placed in the example data directory

## Step-by-step Guide
1. **Prepare the environment** – Ensure the required .NET runtime and Aspose.Imaging library are referenced in your project.  
2. **Locate the source file** – Build the full path to `input-BigTiff.tif` using your data directory.  
3. **Load the image** – Call `Image.Load` and cast the result to `BigTiffImage`.  
4. **Save with options** – Use `BigTiffOptions` (e.g., `TiffExpectedFormat.TiffLzwRgba`) to save the image as a regular TIFF file.  
5. **Clean up** – Delete the generated output file if you only need to demonstrate the conversion process.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "e157cf108f41631a8ba30e78d569dea9" "BigTiffLoadExample.cs" >}}

## See Also
- Converting TIFF images with Aspose.Imaging
- Working with image options and codecs
- Handling large image files in .NET
