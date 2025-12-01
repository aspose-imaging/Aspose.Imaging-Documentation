---
title: Using the Magic Wand Tool to Create and Manipulate Image Masks
linktitle: Magic Wand Tool
type: docs
weight: 30
url: /net/magic-wand-tool/
description: Demonstrates how to use Aspose.Imaging's MagicWandTool to build, combine, and apply image masks.
keywords: magic wand mask c#
---

# Using the Magic Wand Tool to Create and Manipulate Image Masks

## Introduction
This example shows how to employ the **MagicWandTool** from Aspose.Imaging for .NET to generate image masks based on pixel tones, combine them with various operations, feather the result, and finally apply the mask to an image. Use it when you need precise region selection and manipulation without manual drawing.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Input PNG file (`src.png`) placed in the example data directory

## Step-by-step Guide
1. Load the source PNG image as a `RasterImage`.
2. Create an initial mask using `MagicWandTool.Select` with coordinates of a reference pixel.
3. Combine masks using fluent methods:
   - `Union` to add another region.
   - `Invert` to flip the mask.
   - `Subtract` to remove regions or apply a threshold.
4. Remove rectangular areas with consecutive `Subtract` calls that accept `RectangleMask` objects.
5. Feather the mask with `GetFeathered` to soften edges.
6. Apply the final mask to the image via `Apply`.
7. Save the processed image (`result.png`) and clean up.

## Code Example
The full example code is provided below.

{{< gist "aspose-imaging-gists" "086de41b1c8b059d902ee9885527707a" "MagicWandTool.cs" >}}

## See Also
- **Applying Image Filters** – how to add visual effects to images after masking.
- **Working with Raster Images** – basic loading, editing, and saving of raster formats.
- **Image Conversion Basics** – converting between different image types using Aspose.Imaging.
