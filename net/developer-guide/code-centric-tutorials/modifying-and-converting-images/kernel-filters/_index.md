---
title: Applying Kernel Filters to Images with Aspose.Imaging for .NET
linktitle: Kernel Filters
type: docs
weight: 30
url: /net/kernel-filters/
description: Demonstrates how to apply various convolution, deconvolution, and Wiener filters to PNG images using Aspose.Imaging.
keywords: kernel filters c# image processing
---

# Applying Kernel Filters to Images

## Introduction
This example shows how to use Aspose.Imaging for .NET to apply a collection of kernel‑based filters—including convolution, deconvolution, and Wiener filters—to PNG images. It is useful when you need to experiment with different filtering techniques in a single workflow.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample PNG image (e.g., `template.png`) placed in the data directory used by the example

## Step-by-step Guide
1. **Prepare the data directory** – Locate the folder that contains the source PNG image.
2. **Create filter kernels** – Define the size, sigma, and angle for standard kernels and generate a random custom kernel.
3. **Instantiate filter options** – Build an array of `FilterOptionsBase` objects for various filters such as emboss, sharpen, Gaussian blur, deconvolution, and Wiener filters.
4. **Iterate over the source image** – Load the PNG image, apply each filter option, and save the filtered result with a unique file name.
5. **Handle vector images** – If the source is a vector image, convert it to PNG temporarily before applying the raster filters, then clean up temporary files.

## Code Example
The following snippet demonstrates the full workflow:

{{< gist "aspose-imaging-gists" "d97b67e3ab4d19a0c9884ed29bde47fa" "KernelFilters.cs" >}}

## See Also
- Applying Gaussian Blur with Aspose.Imaging
- Sharpening Images Using Convolution Filters
- Converting Between Raster and Vector Formats in Aspose.Imaging
