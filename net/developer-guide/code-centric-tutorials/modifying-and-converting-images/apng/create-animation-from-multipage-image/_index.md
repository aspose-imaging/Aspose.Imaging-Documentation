---
title: Create an APNG Animation from a Multipage Image
linktitle: Create Animation from Multipage Image
type: docs
weight: 30
url: /net/create-animation-from-multipage-image/
description: Creates an APNG animation from a multipage TIFF image using Aspose.Imaging for .NET.
keywords: apng animation c#
---

# Create an APNG Animation from a Multipage Image

## Introduction
This example demonstrates how to generate an animated APNG file from a multipage image (e.g., a TIFF file) using Aspose.Imaging for .NET. It is useful when you need to convert a sequence of frames into a single animated PNG with a defined frame duration.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library installed
- A multipage image file (e.g., `img4.tif`) placed in the sample data directory

## Step-by-step Guide
1. Locate the input multipage image file in the data directory.  
2. Load the image using `Image.Load`.  
3. Create an `ApngOptions` instance and set `DefaultFrameTime` to the desired frame duration (e.g., 500 ms).  
4. Save the loaded image to an APNG file using the options defined in step 3.  
5. (Optional) Delete the generated file after verification.

## Code Example
The following code snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "d7ca5eda87507ce948eceef58b808eab" "CreateAnimationFromMultipageImage.cs" >}}

## See Also
- **Converting a Multipage Image to a Single PNG** – Learn how to extract a single frame from a multipage document.  
- **Working with APNG Options** – Explore additional settings such as loop count and frame-specific timings.  
- **Saving Images in Different Formats** – General guidance on saving images to various formats supported by Aspose.Imaging.
