---
title: Using Optimization Strategy in Resize Operation
linktitle: Optimization Strategy in Resize
type: docs
weight: 30
url: /net/optimization-strategy-in-resize/
description: Demonstrates how to limit memory usage while resizing an image with Aspose.Imaging for .NET.
keywords: resize memory c#
---

# Using Optimization Strategy in Resize Operation

## Introduction
This example shows how to apply a memory optimization strategy when resizing an image. By setting a memory limit during loading, you can control the amount of RAM used, which is especially useful for processing large images on memory‑constrained environments.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A sample TIFF image (e.g., `SampleTiff1.tiff`) placed in the data directory

## Step-by-step Guide
1. **Prepare the data directory** – Obtain the path where the sample image resides.
2. **Load the image with a memory limit** – Use `Image.Load` with `LoadOptions` and set `BufferSizeHint` to the desired limit (e.g., 50 MB).
3. **Resize the image** – Call `image.Resize` with the target width, height, and a resampling type such as `ResizeType.LanczosResample`.
4. **Save the resized image** – Write the output file to the data directory.
5. **Verify the result** – The resized image should be saved with reduced memory footprint during processing.

## Code Example
Below is the complete code for the example:

{{< gist "aspose-imaging-gists" "b510f0e0afd1566997cf3ae2bfcb087e" "OptimizationStrategyInResize.cs" >}}

## See Also
- Resizing Images with Aspose.Imaging
- Controlling Memory Usage with `LoadOptions.BufferSizeHint`
- Working with TIFF Files in Aspose.Imaging
