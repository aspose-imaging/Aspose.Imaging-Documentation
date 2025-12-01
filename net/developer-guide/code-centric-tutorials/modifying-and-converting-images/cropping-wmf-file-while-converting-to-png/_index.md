---
title: Crop a WMF File While Converting to PNG
linktitle: Crop WMF to PNG
type: docs
weight: 30
url: /net/cropping-wmf-file-while-converting-to-png/
description: Demonstrates how to crop a WMF image and save it as a PNG using Aspose.Imaging for .NET.
keywords: crop wmf png
---

# Crop a WMF File While Converting to PNG

## Introduction
This example shows how to load a WMF (Windows Metafile) image, apply a rectangular crop, and then convert the cropped region to a PNG file. Use it when you need to extract a specific area from a vector image and save it in a raster format.

## Prerequisites
- .NET 6.0 or later (compatible with the Aspose.Imaging for .NET library)
- Aspose.Imaging for .NET installed (NuGet package `Aspose.Imaging`)
- Sample WMF file (`File.wmf`) placed in the example data folder

## Step-by-step Guide
1. **Set the data directory** – Locate the folder that contains the sample WMF file.  
2. **Load the WMF image** – Use `Image.Load` to read the WMF file into a `WmfImage` object.  
3. **Apply cropping** – Call `WmfImage.Crop` with a `Rectangle` defining the area to keep.  
4. **Configure rasterization options** – Create a `WmfRasterizationOptions` instance, set background color, page width, and height.  
5. **Create PNG saving options** – Instantiate `PngOptions` and assign the rasterization options via its `VectorRasterizationOptions` property.  
6. **Save the image** – Call `image.Save` with the PNG options to write the cropped content to a PNG file.  
7. **Dispose resources** – The `using` block ensures proper cleanup of the `WmfImage` instance.

## Code Example
The following snippet contains the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "a8a9e6e02cd79c2ab1886dd3c115ad7e" "CroppingWMFfileWhileConvertingtoPNG.cs" >}}

## See Also
- **Converting WMF to JPEG** – Learn how to rasterize WMF files directly to JPEG format.  
- **Resizing and Scaling Images** – Explore resizing techniques for raster images with Aspose.Imaging.  
- **Working with Vector Graphics** – General guide on handling vector formats such as EMF, SVG, and WMF.
