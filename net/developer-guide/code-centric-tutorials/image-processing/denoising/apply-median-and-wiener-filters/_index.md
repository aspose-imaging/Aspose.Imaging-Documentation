---
title: Apply Median and Wiener Filters to an Image
linktitle: Median & Wiener Filters
type: docs
weight: 40
url: /net/apply-median-and-wiener-filters/
description: Demonstrates how to apply median and Wiener filters to reduce noise in an image using Aspose.Imaging for .NET.
keywords: median filter, wiener filter, denoise image
---

# Apply Median and Wiener Filters to an Image

## Introduction
This example shows how to use Aspose.Imaging for .NET to apply median and Wiener filters for noise reduction. It is useful when you need to improve the visual quality of noisy raster images such as GIFs or PNGs.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample noisy image file (e.g., `asposelogo.gif`) placed in the example data directory

## Step-by-step Guide
1. **Locate the data directory** – Use the helper method `RunExamples.GetDataDir_ModifyingAndConvertingImages()` to get the path to the folder containing the input image.  
2. **Load the image** – Call `Image.Load` with the full path to the noisy image.  
3. **Cast to `RasterImage`** – The filtering operations work on raster images, so cast the loaded image accordingly.  
4. **Configure the Median filter** – Create an instance of `MedianFilterOptions`, specifying the kernel size (e.g., `4`).  
5. **Apply the filter** – Invoke `rasterImage.Filter` with the image bounds and the filter options.  
6. **Save the result** – Store the filtered image to a new file (e.g., `median_test_denoise_out.gif`).  

> *Note:* The same approach can be extended to Wiener filters by using the appropriate `WienerFilterOptions` class.

## Code Example
The following snippet contains the complete example. Replace the placeholder with the actual code from the repository.

{{< gist "aspose-imaging-gists" "72d7ea5b661d51bb70913d7f13029d3a" "ApplyMedianAndWienerFilters.cs" >}}

## See Also
- [Applying Gaussian Blur Filter](/net/applying-gaussian-blur-filter/)
- [Reducing Image Noise with Bilateral Filter](/net/bilateral-filter-noise-reduction/)
- [Converting Image Formats](/net/convert-image-formats/)
