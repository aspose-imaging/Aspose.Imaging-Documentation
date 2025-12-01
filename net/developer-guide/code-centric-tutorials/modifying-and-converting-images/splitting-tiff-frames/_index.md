---
title: Splitting Multi-Frame TIFF into Separate Images
linktitle: Splitting TIFF Frames
type: docs
weight: 30
url: /net/splitting-tiff-frames/
description: Demonstrates how to split a multi-frame TIFF into individual frames using Aspose.Imaging for .NET.
keywords: tiff split c#
---

# Splitting TIFF Frames

## Introduction
This example shows how to extract each frame from a multi‑frame TIFF file and save them as separate TIFF images. Use it when you need to work with individual pages of a TIFF document or process them separately.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A source TIFF file containing multiple frames (e.g., `SampleTiff1.tiff`)

## Step-by-step Guide
1. **Locate the source TIFF** – Determine the path to the multi‑frame TIFF you want to split.  
2. **Load the image** – Use `Image.Load` to open the TIFF as a `TiffImage`.  
3. **Iterate through frames** – Access the `Frames` collection of the loaded image.  
4. **Save each frame** – For every frame, call `Save` with a new file name and appropriate `TiffOptions`.  
5. **Dispose resources** – Ensure the `TiffImage` instance is disposed (e.g., via a `using` block) to release file handles.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "f6899572dec565b5543b1e3a28eeade8" "SplittingTiffFrames.cs" >}}

## See Also
- Converting images between formats with Aspose.Imaging
- Working with multi-page TIFF documents
- Basic image manipulation using Aspose.Imaging for .NET
