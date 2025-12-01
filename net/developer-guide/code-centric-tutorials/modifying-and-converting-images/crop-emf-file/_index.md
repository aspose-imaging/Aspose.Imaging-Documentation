---
title: Crop an EMF File using Aspose.Imaging for .NET
linktitle: Crop EMF File
type: docs
weight: 30
url: /net/crop-emf-file/
description: Demonstrates how to crop an EMF image and save the result.
keywords: crop emf image c#
---

# Crop an EMF File using Aspose.Imaging for .NET

## Introduction
This example shows how to load an EMF (Enhanced Metafile) image, crop a specific rectangular region, and save the cropped image as a new EMF file. Use it when you need to extract a portion of an existing vector image without rasterizing it.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An EMF file named `test.emf` placed in the example data directory

## Step-by-step Guide
1. **Set up the data directory** – Obtain the path to the folder containing `test.emf`.
2. **Load the EMF image** – Use `Image.Load` and cast the result to `EmfImage`.
3. **Define the crop rectangle** – Create a `Rectangle` with the desired X, Y, width, and height.
4. **Perform the crop** – Call `image.Crop(rectangle)`.
5. **Save the result** – Save the modified image to a new file, e.g., `test.emf_crop.emf`.
6. **Verify dimensions (optional)** – Output the new width and height to the console for confirmation.

## Code Example
The following code demonstrates the entire process:

{{< gist "aspose-imaging-gists" "625d8423447e3e64fe9829cf2ea1aa5a" "CropEMFFile.cs" >}}

## See Also
- [Resize an EMF Image](../resize-emf-image)
- [Convert EMF to PNG](../convert-emf-to-png)
- [Working with Vector Images in Aspose.Imaging](../vector-image-overview)
