---
title: Apply Bradley Threshold Binarization to an Image
linktitle: Bradley Threshold
type: docs
weight: 30
url: /net/bradleythreshold/
description: Demonstrates how to binarize an image using the Bradley threshold algorithm with Aspose.Imaging for .NET.
keywords: bradley threshold image c#
---

# Apply Bradley Threshold Binarization to an Image

## Introduction
This example shows how to convert a grayscale bitmap into a binary image using the Bradley thresholding technique. Use it when you need adaptive binarization for images with varying lighting conditions.

## Prerequisites
- .NET 6.0 or later (compatible with .NET 9.0)
- Aspose.Imaging for .NET library
- A sample bitmap file (`sample.bmp`) placed in the example data folder

## Step-by-step Guide
1. **Locate the source image** – Define the path to the bitmap you want to process.  
2. **Load the image** – Use `Image.Load` to read the bitmap as a `BmpImage` object.  
3. **Set the threshold value** – Choose a double value (e.g., `0.15`) that determines the sensitivity of the Bradley algorithm.  
4. **Apply Bradley binarization** – Call the `BinarizeBradley` method on the loaded image, passing the threshold value.  
5. **Save the result** – Write the binarized output to a new file, such as `binarized_out.png`.  
6. **Dispose resources** – The `using` block automatically releases the image resources.

## Code Example
The complete source code for this example is provided below.

{{< gist "aspose-imaging-gists" "2678a105d937f208697c6ba25c1e6922" "Bradleythreshold.cs" >}}

## See Also
- [Perform Image Cropping with Aspose.Imaging for .NET](#)
- [Convert BMP to PNG Using Aspose.Imaging for .NET](#)
- [Adjust Image Brightness and Contrast Programmatically](#)
