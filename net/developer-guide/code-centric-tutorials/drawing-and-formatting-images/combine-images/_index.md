---
title: Combine Multiple Images into a Single Canvas
linktitle: Combine Images
type: docs
weight: 30
url: /net/combine-images/
description: Combines two bitmap images into a single JPEG canvas using Aspose.Imaging for .NET.
keywords: combine images c#
---

# Combine Multiple Images into a Single Canvas

## Introduction
This example demonstrates how to merge two bitmap images onto a single canvas and save the result as a JPEG file. It is useful when you need to create composite images, such as photo collages or combined graphics, without manually editing each image.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input bitmap files (`sample_1.bmp` and `File1.bmp`) placed in the example data directory

## Step-by-step Guide
1. **Prepare the output options** – Create a `JpegOptions` instance and set a `FileCreateSource` that points to the desired output file path.
2. **Create a canvas** – Use `Image.Create` with the JPEG options to define a new image canvas of the required width and height (e.g., 600 × 600 pixels).
3. **Initialize graphics** – Obtain a `Graphics` object from the canvas, clear the background (e.g., white), and draw each source bitmap onto specific regions of the canvas using `Graphics.DrawImage`.
4. **Save the result** – Call `image.Save()` to write the combined image to the file system.

## Code Example
The following snippet shows the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "12cc627520b497a70957db3c128a5241" "CombineImages.cs" >}}

## See Also
- **Drawing Images on a Canvas** – Learn how to position and transform images using the `Graphics` class.  
- **Saving Images in Different Formats** – Explore how to save images as PNG, BMP, TIFF, and more with Aspose.Imaging.  
- **Working with Image Sources** – Understand various source types (file, stream, memory) for creating and loading images.
