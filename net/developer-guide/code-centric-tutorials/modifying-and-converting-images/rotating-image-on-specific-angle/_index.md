---
title: Rotate an Image on a Specific Angle with Aspose.Imaging for .NET
linktitle: Rotate Image on Specific Angle
type: docs
weight: 30
url: /net/rotating-image-on-specific-angle/
description: Demonstrates how to rotate an image by a specific angle using Aspose.Imaging for .NET.
keywords: rotate image c#
---

# Rotate an Image on a Specific Angle

## Introduction
This example shows how to rotate an image by a user‑defined angle while preserving its dimensions. It is useful when you need to orient graphics programmatically, such as adjusting logos or preparing images for layout compositions.

## Prerequisites
- .NET 9.0 (or a later compatible version)
- Aspose.Imaging for .NET library
- An input image file (e.g., `aspose-logo.jpg`) placed in the example data directory

## Step-by-step Guide
1. Locate the directory that contains the source image.
2. Load the image into a `RasterImage` instance using `Image.Load`.
3. Ensure the image data is cached for optimal performance (`image.CacheData()` if not already cached).
4. Call `image.Rotate` with the desired angle, enable size proportionality, and specify a background color (e.g., `Color.Red`).
5. Save the rotated image to a new file.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "afd33a28f500132c0c0c5305a13868f0" "RotatingImageOnSpecificAngle.cs" >}}

## See Also
- **Rotating an Image with a Transparent Background** – learn how to rotate while keeping the background transparent.  
- **Scaling and Resizing Images** – explore resizing images proportionally using Aspose.Imaging.  
- **Working with Raster Images** – an overview of raster image handling and manipulation techniques.
