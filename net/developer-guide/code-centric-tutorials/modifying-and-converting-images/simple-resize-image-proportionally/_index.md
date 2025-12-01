---
title: Resize an Image Proportionally Using Aspose.Imaging for .NET
linktitle: Proportional Image Resize
type: docs
weight: 30
url: /net/simple-resize-image-proportionally/
description: Demonstrates how to resize an image proportionally by width or height with Aspose.Imaging for .NET.
keywords: resize image c#
---

# Resize an Image Proportionally

## Introduction
This example shows how to resize an image while maintaining its aspect ratio using the Aspose.Imaging for .NET API. It is useful when you need to scale images down or up without distortion.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An input image file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Load the source image using `Image.Load`.
2. Ensure the image data is cached if required.
3. Calculate the new width (or height) based on the desired scaling factor.
4. Call `ResizeWidthProportionally` or `ResizeHeightProportionally` to adjust the image size while preserving the aspect ratio.
5. Save the resized image to the desired output format.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "4475fec6a811b999c9a4d8d3124e74a0" "SimpleResizeImageProportionally.cs" >}}

## See Also
- [Changing Image Format](#)
- [Applying Image Filters](#)
- [Batch Processing Images](#)
