---
title: Resize WMF File to PNG using Aspose.Imaging for .NET
linktitle: Resize WMF File
type: docs
weight: 30
url: /net/resize-wmf-file/
description: Resizes a WMF image and converts it to a PNG file.
keywords: wmf resize c#
---

# Resize WMF File to PNG

## Introduction
This example demonstrates how to load a WMF image, resize it, and convert the result to a PNG file using Aspose.Imaging for .NET. Use it when you need to rasterize vector WMF graphics at a specific size for web or document workflows.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An input WMF file named **input.wmf** placed in the example data directory

## Step-by-step Guide
1. Initialize the data directory path that contains the source WMF file.  
2. Load the WMF image with `Image.Load`.  
3. Call `image.Resize(width, height)` to set the desired dimensions.  
4. Compute the aspect ratio to maintain proportional height.  
5. Configure `WmfRasterizationOptions` (background color, page size, borders).  
6. Create a `PngOptions` instance and assign the rasterization options.  
7. Save the rasterized image as a PNG file using `image.Save`.  

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "bf7fb3b3d2fbd53ba1732737d079610f" "ResizeWMFFile.cs" >}}

## See Also
- Converting Vector Images to Raster Formats  
- Working with Image Resizing and Scaling Options  
- Saving Images in Different Formats with Aspose.Imaging
