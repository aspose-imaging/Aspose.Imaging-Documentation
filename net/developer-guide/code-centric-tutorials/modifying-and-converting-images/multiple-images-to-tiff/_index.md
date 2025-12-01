---
title: Create a Multi‑Page TIFF from Multiple Images
linktitle: Multiple Images to TIFF
type: docs
weight: 30
url: /net/multiple-images-to-tiff/
description: Combine several images into a single multi‑page TIFF using Aspose.Imaging for .NET.
keywords: tiff c# aspose-imaging
---

# Create a Multi‑Page TIFF from Multiple Images

## Introduction
This example demonstrates how to merge several individual images into one multi‑page TIFF file. Use it when you need to bundle related images (e.g., scanned documents) into a single TIFF document for easier distribution or archiving.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A folder containing the source images (e.g., PNG files) that will be combined

## Step-by-step Guide
1. **Set up the data directory** – Obtain the path where the source images are stored.
2. **Load a sample image** – Use it to determine the width and height for all pages.
3. **Create TIFF options** – Configure `TiffOptions` with the desired format and output file location.
4. **Instantiate a multi‑page TIFF image** – Call `Image.Create` with the TIFF options and the common dimensions.
5. **Iterate over source images**  
   - Load each image.  
   - Resize it to match the target dimensions.  
   - For the first image, use the existing frame; for subsequent images, add a new `TiffFrame`.  
   - Copy pixel data from the source image into the corresponding TIFF frame.
6. **Save the resulting TIFF** – Persist the multi‑page file to the output path.

## Code Example
Below is the complete code snippet illustrating the process:

{{< gist "aspose-imaging-gists" "e2ee2398058a539d3e0a9e168de5585c" "MultipleImagesToTIFF.cs" >}}

## See Also
- **Convert Image Format** – Learn how to convert a single image to another format using Aspose.Imaging.  
- **Resize Images** – Explore image resizing techniques and options.  
- **Work with TIFF Frames** – Detailed guide on adding, removing, and manipulating frames in a TIFF document.
