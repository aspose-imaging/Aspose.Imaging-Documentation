---
title: Applying a PNG Filter Method
linktitle: Apply PNG Filter
type: docs
weight: 30
url: /net/apply-filter-method/
description: Demonstrates how to set a PNG filter method and save the image using Aspose.Imaging for .NET.
keywords: png filter c#
---

# Applying a PNG Filter Method

## Introduction
This example shows how to change the filter method applied to a PNG image and save the result. Use it when you need to control PNG compression behavior for better compatibility or optimized file size.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- A PNG image file (e.g., `aspose_logo.png`) placed in the data folder used by the examples

## Step-by-step Guide
1. Obtain the path to the folder that contains the source PNG image.  
2. Load the PNG image using `Image.Load` and cast it to `PngImage`.  
3. Create a `PngOptions` instance.  
4. Set the `FilterType` property of the options to the desired filter method (e.g., `PngFilterType.Paeth`).  
5. Save the image with the configured options to a new file.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "3790cc3ee64ca2753d0e89f3f94fe2c2" "ApplyFilterMethod.cs" >}}

## See Also
- Converting PNG images to other formats
- Using additional PNG options (e.g., interlacing, bit depth)
- Applying image filters and effects with Aspose.Imaging for .NET
