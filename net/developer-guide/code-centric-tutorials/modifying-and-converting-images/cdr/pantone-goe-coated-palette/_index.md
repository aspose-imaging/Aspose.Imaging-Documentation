---
title: Convert CDR Image to PNG Using Pantone Goe Coated Palette
linktitle: Pantone Goe Coated Palette
type: docs
weight: 30
url: /net/pantone-goe-coated-palette/
description: Demonstrates loading a CDR file and saving it as PNG with Pantone Goe Coated rasterization options using Aspose.Imaging for .NET.
keywords: cdr png conversion
---

# Convert CDR Image to PNG Using Pantone Goe Coated Palette

## Introduction
This example shows how to load a CorelDRAW (CDR) image, apply Pantone Goe Coated rasterization settings, and save the result as a PNG file. Use it when you need to convert CDR drawings to raster formats while preserving specific color profiles.

## Prerequisites
- .NET 9.0 (or later compatible version)
- Aspose.Imaging for .NET library
- A sample CDR file (`test2.cdr`) placed in the example data folder

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path where example assets are stored.  
2. **Load the CDR image** – Use `Image.Load` to read the `.cdr` file as a `CdrImage`.  
3. **Configure PNG options** – Create `PngOptions` with a `CdrRasterizationOptions` object, setting `Positioning` to `Relative` to apply the Pantone Goe Coated palette.  
4. **Save the image** – Export the rasterized image to `result.png` using the configured options.  
5. **Clean up** – Delete the generated PNG file after verification (optional).

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "84ceeb3cd3d6ffa946811bdf70309dbc" "PantoneGoeCoatedPalette.cs" >}}

## See Also
- Converting CDR to JPEG with custom rasterization  
- Working with color palettes in vector-to-raster conversion  
- Loading and saving images with Aspose.Imaging for .NET
