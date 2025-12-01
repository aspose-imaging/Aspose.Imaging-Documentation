---
title: Export APNG to GIF using Aspose.Imaging for .NET
linktitle: Export APNG to GIF
type: docs
weight: 30
url: /net/export-apng-to-gif/
description: Demonstrates how to convert an animated PNG (APNG) to an animated GIF with Aspose.Imaging for .NET.
keywords: apng gif conversion c#
---

# Export APNG to GIF

## Introduction
This example shows how to load an animated PNG (APNG) file and export it as an animated GIF using Aspose.Imaging for .NET. Use it when you need to convert APNG assets to GIF format for broader compatibility in web or application scenarios.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- An APNG file (e.g., `elephant.png`) placed in the example data directory

## Step-by-step Guide
1. **Prepare the environment** – Ensure the required .NET runtime and Aspose.Imaging package are referenced in your project.  
2. **Locate the source APNG** – Build the full path to the APNG file you want to convert.  
3. **Load the image** – Use `Image.Load` to read the APNG into an `Image` object.  
4. **Save as GIF** – Call `image.Save` with a `GifOptions` instance to export the animation to a GIF file.  
5. **Clean up (optional)** – Delete the generated GIF file if you only need to verify the conversion during the example run.

## Code Example
The snippet below demonstrates the conversion process:

{{< gist "aspose-imaging-gists" "c7ff17f0ec19f4bade69392bb3f246b8" "ExportAPNGToGif.cs" >}}

## See Also
- Converting other image formats to GIF  
- Working with APNG images in Aspose.Imaging  
- Saving images with custom options (e.g., PNG, JPEG, BMP)
