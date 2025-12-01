---
title: Automatic Background Removal Using Graph Cut
linktitle: Graph Cut Auto Masking
type: docs
weight: 20
url: /net/graph-cut-auto-masking/
description: Demonstrates how to automatically remove an image background with the Graph Cut algorithm.
keywords: background removal, graph cut, c#
---

# Remove Image Background Using Graph Cut

## Introduction
This example shows how to automatically isolate and remove the background of a JPEG image by leveraging Aspose.Imaging's Graph Cut segmentation. Use it when you need a quick, high‑quality mask without manually drawing strokes.

## Prerequisites
- .NET 6.0 or later  
- Aspose.Imaging for .NET library installed  
- An input JPEG image (e.g., `input.jpg`) placed in the example data folder

## Step-by-step Guide
1. Load the source image with `Image.Load`.  
2. Create `AutoMaskingGraphCutOptions` and configure:
   - Enable automatic stroke calculation  
   - Set feathering radius relative to image size  
   - Choose `SegmentationMethod.GraphCut`  
   - Provide PNG export options for an alpha‑channel output  
3. Run the segmentation using `new ImageMasking(image).Decompose(options)`.  
4. Retrieve the mask image (usually the second result) and save it as a PNG with transparency.  
5. (Optional) Delete the temporary PNG if you only need the mask data.

## Code Example
Below is the complete source code for the example:

{{< gist "aspose-imaging-gists" "617e8e7c69c9bcaced82c71cc514e65d" "GraphCutAutoMasking.cs" >}}

## See Also
- **Manual Image Masking** – Learn how to define custom strokes for mask creation.  
- **Color-Based Background Removal** – Remove backgrounds using color similarity criteria.  
- **Saving Images with Transparency** – Explore options for exporting images with an alpha channel.
