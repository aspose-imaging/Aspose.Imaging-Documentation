---
title: Support of FODG – Convert ODG to PNG with Vector Rasterization
linktitle: Support of FODG
type: docs
weight: 30
url: /net/support-of-fodg/
description: Demonstrates how to load an FODG file and save it as PNG using vector rasterization.
keywords: FODG conversion C#
---

# Support of FODG – Convert ODG to PNG with Vector Rasterization

## Introduction
This example shows how to load a **FODG** (Free Open Design Graph) file and rasterize it into a PNG image using Aspose.Imaging for .NET.  
Use it when you need to render vector‑based ODG graphics as raster images for web or reporting scenarios.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample `sample.fodg` file placed in the example data folder

## Step-by-step Guide
1. **Locate the source file** – Retrieve the path to the `sample.fodg` file using the helper method `RunExamples.GetDataDir_OTG()`.  
2. **Load the image** – Call `Image.Load` with the ODG file path to obtain an `Image` object.  
3. **Configure rasterization options** – Create a `PngOptions` instance and set its `VectorRasterizationOptions` to an `OdgRasterizationOptions` object, specifying the page size based on the original image dimensions.  
4. **Save as PNG** – Use `image.Save` with the output filename (`sample.fodg.png`) and the configured `PngOptions`.  
5. **Dispose resources** – The `using` statement automatically releases the image resources after saving.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "f5064ee815a6808c85e22cf0ba307251" "SupportOfFODG.cs" >}}

## See Also
- **Convert SVG to PNG** – Learn how to rasterize SVG files with custom dimensions.  
- **Working with Vector Images** – Overview of vector image support in Aspose.Imaging.  
- **Image Loading and Saving Options** – Detailed guide on the various image formats and options available.
