---
title: Improving Default Font Usage When Converting ODG to PNG
linktitle: Default Font Usage Improve
type: docs
weight: 30
url: /net/default-font-usage-improve/
description: Demonstrates how to set a default font and improve missing‑font handling during ODG to PNG conversion.
keywords: default-font otg png
---

# Improving Default Font Usage When Converting ODG to PNG

## Introduction
This example shows how to handle missing fonts when converting ODG files to PNG images using Aspose.Imaging for .NET. By configuring the `FontSettings` you can specify a fallback font and improve the rendering quality of documents that reference unavailable fonts.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample ODG files and a `fonts` folder containing the desired fallback fonts

## Step-by-step Guide
1. Locate the data directory that contains the ODG source file and the `fonts` sub‑folder.  
2. Set the custom fonts folder with `FontSettings.SetFontsFolder`.  
3. Disable system alternative fonts by setting `FontSettings.GetSystemAlternativeFont` to `false`.  
4. For each required fallback font, assign `FontSettings.DefaultFontName` and load the ODG file via `Image.Load`.  
5. Configure `PngOptions` with appropriate `VectorRasterizationOptions` (e.g., page width and height).  
6. Save the image as PNG, then optionally delete the temporary output file.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "5a367189a140bfd764272a8b48c7e3f8" "DefaultFontUsageImprove.cs" >}}

## See Also
- Converting ODG to PNG with Aspose.Imaging
- Working with `FontSettings` in Aspose.Imaging
- Rasterizing vector images using `VectorRasterizationOptions`
