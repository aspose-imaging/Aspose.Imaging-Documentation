---
title: Resize Images Using Aspose.Imaging for .NET
linktitle: Simple Resizing
type: docs
weight: 30
url: /net/simple-resizing/
description: Demonstrates how to resize images and apply different resize types with Aspose.Imaging for .NET.
keywords: resizing image c#
---

# Simple Resizing Example

## Introduction
This example shows how to resize an image to specific dimensions and how to use a high‑quality resize algorithm with Aspose.Imaging for .NET. Use it when you need to generate thumbnails or adapt images to fit particular layout requirements.

## Prerequisites
- .NET 6.0 or later (compatible with your project)
- Aspose.Imaging for .NET library
- Sample image file (e.g., `aspose-logo.jpg`) placed in the project’s data directory

## Step-by-step Guide
1. Load the source image using `Image.Load`.
2. Call `Resize(width, height)` to shrink or enlarge the image to the desired size.
3. Save the resized image to a new file.
4. (Optional) Reload the image and call `Resize(width, height, ResizeType.CatmullRom)` to apply a high‑quality Catmull‑Rom resampling algorithm.

## Code Example
Below is the complete code for the Simple Resizing example:

{{< gist "aspose-imaging-gists" "41675e24508a113baa83bad1eba01064" "SimpleResizing.cs" >}}

## See Also
- **Image Format Conversion** – Learn how to convert images between different formats.
- **Advanced Image Manipulation** – Explore cropping, rotating, and applying filters.
- **Working with Streams** – Understand how to load and save images using streams for better performance.
