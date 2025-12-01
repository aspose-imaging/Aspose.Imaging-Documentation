---
title: Support for EPS Format
linktitle: EPS Format Support
type: docs
weight: 30
url: /net/support-for-eps-format/
description: Demonstrates how to load an EPS image and extract its preview images using Aspose.Imaging for .NET.
keywords: eps image c#
---

# Support for EPS Format

## Introduction
This example shows how to work with EPS files using Aspose.Imaging for .NET. It loads an EPS image, extracts all available preview images, and saves them in the appropriate format. Use this when you need to generate thumbnails or preview graphics from EPS documents.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An EPS file (e.g., `sample.eps`) placed in the data directory used by the examples

## Step-by-step Guide
1. Obtain the path to the directory containing the EPS sample file.
2. Load the EPS file with `Image.Load` and cast it to `EpsImage`.
3. Call `GetPreviewImages()` on the loaded image to retrieve a collection of preview images.
4. Iterate through each preview image, construct an output file name based on its format, and save it using `preview.Save`.
5. Optionally, clean up any generated preview files after processing.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "59e7675976f0979d9bf07cd19009ab22" "SupportForEPSFormat.cs" >}}

## See Also
- Converting EPS to Raster Formats
- Working with Image Metadata in Aspose.Imaging
- Generating Thumbnails for Vector Images
