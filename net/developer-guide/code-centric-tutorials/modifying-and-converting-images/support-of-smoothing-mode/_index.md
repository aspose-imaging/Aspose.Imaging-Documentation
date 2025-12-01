---
title: Apply Smoothing Modes When Converting Vector Images
linktitle: Support of Smoothing Mode
type: docs
weight: 30
url: /net/support-of-smoothing-mode/
description: Demonstrates how to use different smoothing modes while converting vector images to PNG with Aspose.Imaging for .NET.
keywords: smoothing mode, vector conversion, C#
---

# Apply Different Smoothing Modes When Converting Vector Images

## Introduction
This example shows how to render vector images (such as CDR, CMX, EMF, WMF, ODG, and SVG) using various `SmoothingMode` settings. By adjusting the smoothing mode you can control the visual quality of the resulting raster image, useful when anti‑aliasing is required or when a faster, non‑smoothed output is preferred.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample vector files: `SmoothingTest.cdr`, `SmoothingTest.cmx`, `SmoothingTest.emf`, `SmoothingTest.wmf`, `SmoothingTest.odg`, `SmoothingTest.svg`

## Step-by-step Guide
1. **Set up the data directory** – Obtain the path to the folder containing the sample vector files.  
2. **Create a list of source files** – Include all supported vector formats you want to process.  
3. **Define smoothing modes** – Use `SmoothingMode.AntiAlias` for high‑quality rendering and `SmoothingMode.None` for faster rendering without anti‑aliasing.  
4. **Load each image** – Call `Image.Load` for every file in the list.  
5. **Create the appropriate rasterization options** – Depending on the image type (`CdrImage`, `CmxImage`, `EmfImage`, `WmfImage`, `OdgImage`, `SvgImage`), instantiate the matching rasterization options class.  
6. **Set page size** – Assign the original image size to `vectorRasterizationOptions.PageSize`.  
7. **Iterate over smoothing modes** – For each mode, update `vectorRasterizationOptions.SmoothingMode` and save the image as PNG using `PngOptions` with the configured rasterization options.  
8. **Verify output** – The generated PNG files will be named `image_<SmoothingMode>_<OriginalFileName>.png`.

## Code Example
The following snippet demonstrates the complete workflow described above:

{{< gist "aspose-imaging-gists" "54fe0685fc3b5f813628891fd7141730" "SupportOfSmoothingMode.cs" >}}

## See Also
- Converting Vector Images to Raster Formats  
- Working with Image Options in Aspose.Imaging  
- Using Rasterization Options for Custom Rendering
