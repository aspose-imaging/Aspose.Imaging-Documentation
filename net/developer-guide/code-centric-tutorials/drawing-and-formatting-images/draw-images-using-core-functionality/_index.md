---
title: Draw Images Using Core Functionality
linktitle: Draw Images
type: docs
weight: 30
url: /net/draw-images-using-core-functionality/
description: Demonstrates how to create and manipulate a BMP image using Aspose.Imaging core functionality.
keywords: draw image c#
---

# Draw Images Using Core Functionality

## Introduction
This example shows how to create a BMP image from scratch, fill it with a solid color, and save the result using Aspose.Imaging for .NET. Use it when you need low‑level pixel manipulation or want to generate bitmap graphics programmatically.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- No external files are required; the example generates the image in memory and saves it to the output folder.

## Step-by-step Guide
1. **Create BMP image options** – instantiate `BmpOptions` and set the desired bits per pixel (e.g., 24).
2. **Define the output source** – use `FileCreateSource` to specify the output file path.
3. **Create a raster image** – call `Image.Create` with the BMP options and the required dimensions (e.g., 500 × 500).
4. **Load the pixel buffer** – retrieve all pixels of the image using `LoadPixels`.
5. **Modify pixel colors** – iterate through the buffer and set each pixel to the desired color (yellow in this case).
6. **Apply changes and save** – use `SavePixels` to write the modified buffer back to the image, then call `Save` to write the file to disk.

## Code Example
The complete source code is shown below:

{{< gist "aspose-imaging-gists" "f5ca59c45061a4d61b08e3babf55e489" "DrawImagesUsingCoreFunctionality.cs" >}}

## See Also
- **Creating Images** – learn how to create images in different formats using Aspose.Imaging.
- **Working with Raster Images** – explore advanced pixel‑level operations and image processing techniques.
- **Saving Images in Various Formats** – see how to export images to PNG, JPEG, TIFF, and other supported formats.
