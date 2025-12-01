---
title: Concatenating TIFF Images from Stream
linktitle: Concatenating TIFF Images
type: docs
weight: 30
url: /net/concatenating-tiff-images-from-stream/
description: Demonstrates how to concatenate multiple TIFF images using streams with Aspose.Imaging for .NET.
keywords: tiff stream c#
---

# Concatenating TIFF Images from Stream

## Introduction
This example shows how to merge (concatenate) two TIFF images by loading them from file streams and adding the source image's frame to the destination image. Use it when you need to combine separate TIFF files without first saving them to disk as separate images.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Two sample TIFF files (`TestDemo.tif` and `sample1.tif`) placed in the example data folder

## Step-by-step Guide
1. Obtain the data directory that contains the source TIFF files.  
2. Open each TIFF file with a `FileStream`.  
3. Load the first stream into a `TiffImage` object—this will be the destination image.  
4. Load the second stream into another `TiffImage` object—this serves as the source image.  
5. Copy the active frame from the source image using `TiffFrame.CopyFrame`.  
6. Add the copied frame to the destination image with `image.AddFrame`.  
7. Save the combined image to a new TIFF file.  
8. Close the file streams to release resources.

## Code Example
The following code demonstrates the entire workflow:

{{< gist "aspose-imaging-gists" "02e673ef2561ab1795b3956f906852a7" "ConcatenatingTIFFImagesfromStream.cs" >}}

## See Also
- [Appending Frames to a Multi-Page TIFF Image](#)
- [Saving Images in Different Formats with Aspose.Imaging](#)
- [Working with TIFF Images in Aspose.Imaging for .NET](#)
