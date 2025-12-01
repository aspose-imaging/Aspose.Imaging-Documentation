---
title: Export Raster Image to SVG using Aspose.Imaging for .NET
linktitle: Export Raster to SVG
type: docs
weight: 30
url: /net/export-raster-image-to-svg/
description: Convert raster images such as GIF, JPEG, PNG, PSD, and WebP to SVG vector format with Aspose.Imaging for .NET.
keywords: svg conversion c#
---

# Export Raster Image to SVG

## Introduction
This example shows how to convert various raster image formats (e.g., GIF, JPEG, PNG, PSD, TIFF, WebP) into scalable SVG files using Aspose.Imaging for .NET. It is useful when you need vector representations of bitmap images for scaling without quality loss.

## Prerequisites
- .NET 6.0 or later (compatible with your project)
- Aspose.Imaging for .NET library installed via NuGet
- Sample raster image files placed in a accessible folder (paths used in the example)

## Step-by-step Guide
1. **Set up the source directory** – Determine the folder that contains the raster images you want to convert.  
2. **Create a list of image paths** – Prepare an array with full paths to each raster image file.  
3. **Iterate through each image** – Loop over the array to process every image individually.  
4. **Load the image** – Use `Image.Load(path)` to read the raster image into memory.  
5. **Configure SVG export options** –  
   - Instantiate `SvgOptions`.  
   - Create `SvgRasterizationOptions` and assign it to `SvgOptions.VectorRasterizationOptions`.  
   - Set `PageWidth` and `PageHeight` to match the original image dimensions.  
6. **Save as SVG** – Call `image.Save(destinationPath, svgOptions)` where `destinationPath` appends “.svg” to the original file name.  
7. **Repeat** – Continue the loop for each image in the list.

## Code Example
The following code demonstrates exporting multiple raster images to SVG format:

{{< gist "aspose-imaging-gists" "d0faab2a62cd2c1bb5aba0596f911772" "ExportRasterImageToSvg.cs" >}}

## See Also
- Converting images to PDF with Aspose.Imaging for .NET  
- Rasterizing vector graphics to bitmap using Aspose.Imaging  
- Working with PSD files in Aspose.Imaging for .NET
