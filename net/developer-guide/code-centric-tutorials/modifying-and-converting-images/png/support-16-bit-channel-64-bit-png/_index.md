---
title: Support 16‑Bit Channel 64‑Bit PNG
linktitle: 16‑Bit Channel PNG
type: docs
weight: 30
url: /net/support-16-bit-channel-64-bit-png/
description: Demonstrates how to load and save a 16‑bit per channel PNG using Aspose.Imaging for .NET.
keywords: png,16-bit,c#
---

# Support 16‑Bit Channel 64‑Bit PNG

## Introduction
This example shows how to work with PNG images that have 16‑bit per channel depth, resulting in a 64‑bit total color depth. Use it when you need to preserve high‑precision color information while processing PNG files with Aspose.Imaging for .NET.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample 16‑bit PNG file (provided in the Aspose.Imaging example data set)

## Step-by-step Guide
1. Obtain the data directory that contains the sample PNG image.  
2. Load the PNG image as a `RasterImage` using `Image.Load`.  
3. Retrieve the original image options via `GetOriginalOptions`.  
4. Save the image back to PNG format using the original options to preserve the 16‑bit channel depth.  
5. Optionally delete the generated file to clean up after execution.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "ede6cf5a3aa6fde169d3259448c8d917" "Support16BitChannel64BitPng.cs" >}}

## See Also
- Converting PNG to JPEG with Aspose.Imaging  
- Working with TIFF images in Aspose.Imaging  
- Optimizing image file size using Aspose.Imaging settings
