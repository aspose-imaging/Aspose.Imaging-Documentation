---
title: Automatic Image Masking with Aspose.Imaging for .NET
linktitle: Auto Image Masking
type: docs
weight: 30
url: /net/auto-image-masking/
description: Demonstrates how to automatically mask an image using graph‑cut segmentation.
keywords: auto masking c#
---

# Automatic Image Masking

## Introduction
This example shows how to perform automatic image masking using Aspose.Imaging for .NET. It leverages the GraphCut segmentation method to separate foreground objects from the background, producing a PNG with an alpha channel. Use this approach when you need quick, high‑quality masks without manually defining regions.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Input PNG image and corresponding `.dat` file containing masking points (provided in the Aspose.Imaging examples data folder)

## Step-by-step Guide
1. Set up the data directory that contains the source PNG and the points file.  
2. Load the source image as a `RasterImage`.  
3. Create an `AutoMaskingArgs` instance and populate it with the points from the `.dat` file.  
4. Configure `MaskingOptions`:
   - Set `Method` to `SegmentationMethod.GraphCut`.
   - Assign the prepared `AutoMaskingArgs` to `Args`.
   - Specify PNG export options with truecolor‑with‑alpha format.  
5. Call `new ImageMasking(image).Decompose(maskingOptions)` to generate mask results.  
6. Retrieve the desired masked layer (`maskingResults[1]`) and save it as a PNG file.  
7. Release all resources by disposing objects or using `using` statements.

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "73ad3beec6c47616b7045c809005e4fd" "AutoImageMasking.cs" >}}

## See Also
- **Applying Manual Masks** – learn how to define custom mask regions programmatically.  
- **Converting Images to PNG with Transparency** – explore different ways to add alpha channels during format conversion.  
- **Image Segmentation Techniques** – overview of segmentation methods available in Aspose.Imaging.
