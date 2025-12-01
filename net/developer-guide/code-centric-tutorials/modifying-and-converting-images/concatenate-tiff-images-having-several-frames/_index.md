---
title: Concatenate TIFF Images Having Several Frames
linktitle: Concatenate TIFF Images
type: docs
weight: 30
url: /net/concatenate-tiff-images-having-several-frames/
description: Concatenates multiple multi‑frame TIFF images into a single TIFF file.
keywords: tiff concatenate c#
---

# Concatenate TIFF Images Having Several Frames

## Introduction
This example shows how to merge several TIFF images that contain multiple frames into a single multi‑frame TIFF file. Use it when you need to combine scanned pages or layered TIFF documents while preserving each original frame.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Two or more source TIFF files with one or more frames each

## Step-by-step Guide
1. **Prepare the source files** – Build a list of file paths that point to the TIFF images you want to merge.  
2. **Set TIFF save options** – Create a `TiffOptions` instance and configure properties such as `BitsPerSample`, `Orientation`, `Photometric`, `Compression`, and `FillOrder`.  
3. **Load each TIFF image** – Use `Image.Load` to open each source file as a `TiffImage`.  
4. **Iterate through frames** – For every frame in each loaded image, copy the frame:
   - If the output image has not been created yet, instantiate a new `TiffImage` with the first copied frame.  
   - Otherwise, add the copied frame to the existing output image with `AddFrame`.  
5. **Save the concatenated image** – Call `Save` on the output `TiffImage`, passing the desired file name and the previously configured `TiffOptions`.  
6. **Dispose resources** – Ensure all loaded `TiffImage` objects are disposed to free memory.

## Code Example
The following snippet demonstrates the complete process of concatenating multi‑frame TIFF images:

{{< gist "aspose-imaging-gists" "18f596fba6d942e8d5bf62bd47f6b7e1" "ConcatenateTiffImagesHavingSeveralFrames.cs" >}}

## See Also
- Working with multi‑frame images in Aspose.Imaging
- Saving images in different TIFF compression formats
- Modifying TIFF image properties such as orientation and photometric interpretation
