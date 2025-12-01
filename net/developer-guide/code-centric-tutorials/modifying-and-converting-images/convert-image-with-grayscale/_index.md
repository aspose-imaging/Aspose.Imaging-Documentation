---
title: Convert Image to Grayscale and Save with Different Color Types
linktitle: Convert Image Grayscale
type: docs
weight: 30
url: /net/convert-image-with-grayscale/
description: Demonstrates how to convert a JPEG image to grayscale and other color types using Aspose.Imaging for .NET.
keywords: grayscale image c#
---

# Convert Image to Grayscale and Save with Different Color Types

## Introduction
This example shows how to load a JPEG image, apply various JPEG color modes—including grayscale—and save the results with a custom bit depth. Use it when you need to generate multiple versions of an image for different color requirements.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Sample JPEG image(s) placed in the data directory used by the examples

## Step-by-step Guide
1. **Initialize the data directory** where source images are located.  
2. **Define an array of `JpegCompressionColorMode` values** you want to apply (e.g., Grayscale, YCbCr, Rgb, etc.).  
3. **Create a `JpegOptions` instance** and set the desired `BitsPerChannel` (12 bits in this case).  
4. **Iterate through each color mode**, assign it to `options.ColorType`, generate an appropriate output file name, and save the image using `Image.Save` with the configured options.  
5. **Dispose of the image objects** automatically with a `using` statement to free resources.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "7850a7dd21684c1c466565d85085340c" "ConvertImageWithGrayscale.cs" >}}

## See Also
- Converting an image to different formats
- Changing image color depth and bit depth
- Working with JPEG compression options in Aspose.Imaging
