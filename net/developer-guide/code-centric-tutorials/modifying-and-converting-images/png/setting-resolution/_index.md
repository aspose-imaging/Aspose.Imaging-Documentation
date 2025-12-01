---
title: Setting Image Resolution for PNG Files
linktitle: Setting Resolution
type: docs
weight: 30
url: /net/setting-resolution/
description: Demonstrates how to set horizontal and vertical resolution when saving a PNG image using Aspose.Imaging for .NET.
keywords: png resolution c#
---

# Setting Image Resolution for PNG Files

## Introduction
This example shows how to load a PNG image, copy its pixel data, and save it with custom horizontal and vertical resolution settings. Use this approach when you need precise DPI control for PNG output, such as preparing images for print or specific display requirements.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Input PNG file (e.g., `aspose_logo.png`) placed in the example data folder

## Step-by-step Guide
1. **Load the source PNG image** using `Image.Load` and cast it to `RasterImage` to access pixel data.  
2. **Retrieve image dimensions** (`Width` and `Height`) and load all pixels into a `Color[]` array with `LoadPixels`.  
3. **Create a new `PngImage`** with the same dimensions to serve as the destination image.  
4. **Copy the pixel data** to the new image using `SavePixels`.  
5. **Configure `PngOptions`** and set `ResolutionSettings` to the desired DPI values (e.g., 72 × 96).  
6. **Save the new PNG** with the specified resolution to the output path.

## Code Example
The following snippet contains the complete code for the scenario described above:

{{< gist "aspose-imaging-gists" "3077067f9555800838b7a852b9cfcd99" "SettingResolution.cs" >}}

## See Also
- Loading Pixels from a PNG Image
- Saving PNG with Custom Options
- Changing Image Resolution for JPEG Images
