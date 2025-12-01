---
title: Replacing Missing Fonts When Converting Meta Files
linktitle: Replace Missing Fonts
type: docs
weight: 30
url: /net/support-for-replacing-missing-fonts/
description: Demonstrates how to set a default font and convert EMF/Odg/SVG/WMF files to PNG while handling missing fonts.
keywords: font replacement, meta files, aspose imaging
---

# Replacing Missing Fonts When Converting Meta Files

## Introduction
This example shows how to specify a fallback font and convert various vector meta‑file formats (EMF, ODg, SVG, WMF) to PNG images using Aspose.Imaging for .NET. Use it when the source files reference fonts that are not installed on the processing machine.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample meta‑file assets (e.g., `Fonts.emf`) placed in the example data directory

## Step-by-step Guide
1. Retrieve the path to the example data directory using `RunExamples.GetDataDir_MetaFiles()`.  
2. Set a default font name with `FontSettings.DefaultFontName`. This font will be used when the original font cannot be found.  
3. Create an array of source file names and a matching array of `VectorRasterizationOptions` for each target format (`EmfRasterizationOptions`, `OdgRasterizationOptions`, `SvgRasterizationOptions`, `WmfRasterizationOptions`).  
4. Iterate over the files, load each image with `Image.Load`, configure the rasterization options (page width/height), and save the result as a PNG using `Image.Save` with `PngOptions`.  
5. Verify the output PNG files are generated with the fallback font applied.

## Code Example
The following snippet contains the complete runnable code for this scenario:

{{< gist "aspose-imaging-gists" "c86dbc7289069ba1debce0c5c99befa8" "SupportForReplacingMissingFonts.cs" >}}

## See Also
- **Converting Vector Images to Raster Formats** – Learn how to rasterize other vector formats to raster images.  
- **Working with FontSettings in Aspose.Imaging** – Detailed guide on managing font substitution and embedding.  
- **Saving Images in Different Formats** – Overview of saving images using various `ImageOptions` classes.
