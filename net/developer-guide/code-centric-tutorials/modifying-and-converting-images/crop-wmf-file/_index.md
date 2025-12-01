---
title: Crop a WMF File Using Aspose.Imaging for .NET
linktitle: Crop WMF File
type: docs
weight: 30
url: /net/crop-wmf-file/
description: Demonstrates how to crop a WMF image and save the result with Aspose.Imaging for .NET.
keywords: wmf, crop, c#
---

# Crop a WMF File Using Aspose.Imaging for .NET

## Introduction
This example shows how to load a WMF (Windows Metafile) image, crop a specific region, and save the cropped output. Use it when you need to extract a portion of a vector graphic without converting it to another format.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A WMF source file named `test.wmf` placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the directory that contains the source WMF file.  
2. Load the WMF image using `Image.Load` and cast it to `WmfImage`.  
3. Call the `Crop` method with a `Rectangle` that defines the region to keep (e.g., `new Rectangle(10, 10, 100, 150)`).  
4. Optionally, read the image dimensions after cropping for verification.  
5. Save the cropped image to a new file (e.g., `test.wmf_crop.wmf`).  

## Code Example
The following C# code demonstrates how to crop a WMF image:

{{< gist "aspose-imaging-gists" "723418fb335994bf89fc0f8cbd841ddf" "CropWMFFile.cs" >}}

## See Also
- Converting WMF files to raster formats  
- Resizing images with Aspose.Imaging  
- Working with vector graphics in Aspose.Imaging for .NET
