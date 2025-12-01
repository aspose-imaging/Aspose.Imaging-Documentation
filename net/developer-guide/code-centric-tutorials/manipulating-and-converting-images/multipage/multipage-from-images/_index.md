---
title: Create a Multipage TIFF Image from Multiple Images
linktitle: Multipage from Images
type: docs
weight: 30
url: /net/multipage-from-images/
description: Demonstrates how to combine several images into a single multipage TIFF file using Aspose.Imaging for .NET.
keywords: multipage tiff Aspose
---

# Create a Multipage TIFF Image from Multiple Images

## Introduction
This example shows how to load a collection of different image files and combine them into a single multipage TIFF image. Use it when you need to package multiple graphics (e.g., PNG, GIF, TIFF, CDR) into one file for easier distribution or archival.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A set of source images (e.g., `33266.tif`, `Animation.gif`, `elephant.png`, `MultiPage.cdr`) placed in the example data folder

## Step-by-step Guide
1. **Identify the source folder** that contains the images you want to merge.  
2. **Create a list of image file names** you wish to include in the multipage document.  
3. **Load each image** using `Image.Load` and add it to a `List<Image>`.  
4. **Generate a multipage image** with `Image.Create(imagesArray, true)`.  
5. **Save the result** as a TIFF file using `TiffOptions` with the desired format (e.g., `TiffJpegRgb`).  
6. **Optionally clean up** by deleting the generated TIFF file after verification.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "cf6072d60af07c0377515b0866c2b7a4" "MultipageFromImages.cs" >}}

## See Also
- [Convert Images to Different Formats](#)  
- [Apply Image Filters and Effects](#)  
- [Work with TIFF Features in Aspose.Imaging](#)
