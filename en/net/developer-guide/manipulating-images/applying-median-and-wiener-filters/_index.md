---
title: Applying Median and Wiener Filters - Denoise Image in C#
linktitle: Applying Median and Wiener Filters
type: docs
weight: 20
url: /net/applying-median-and-wiener-filters/
keywords: denoise image c#
description: The median filter is a nonlinear digital filtering technique, often used to remove noise. Using C# Image Processing Library developers can apply median filter to denoise the image and can apply gauss wiener filter on images.
---

## **Applying Median and Wiener Filters**
The median filter is a nonlinear digital filtering technique, often used to remove noise. Such noise reduction is a typical pre-processing step to improve the results of later processing. The Wiener filter is the MSE(mean squared error) optimal stationary linearfilter for images degraded by additive noise and blurring. Using Aspose.Imaging for .NET API developers can apply median filter to denoise the image and can apply gauss wiener filter on images. This article demonstrates how median filter and gauss wiener filter can be applied to images.
### **Applying Median Filter**
Aspose.Imaging provides [Medianfilteroptions](https://reference.aspose.com/imaging/net/aspose.imaging.imagefilters.filteroptions/medianfilteroptions) class to apply filter on a [RasterImage](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage). The code snippet provided below demonstrates how to apply median filter to a raster image.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "apply-median-filter.cs" >}}
### **Applying Gauss Wiener Filter**
Aspose.Imaging provides [GaussWienerFilterOptions](https://reference.aspose.com/imaging/net/aspose.imaging.imagefilters.filteroptions/gausswienerfilteroptions) class to apply filter on a [RasterImage](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage). The code snippet provided below demonstrates how to apply gauss wiener filter to a raster image.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "apply-gauss-weiner-filter.cs" >}}

Applying Gauss Wiener Filter For Colored image

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "apply-gauss-weiner-filter-for-colored-image.cs" >}}
### **Applying Motion Wiener Filter**
Aspose.Imaging provides MotionWienerFilterOptions class to apply filter on a [RasterImage](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage). The code snippet provided below demonstrates how to apply motion wiener filter to a raster image.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "apply-motion-weiner-filter.cs" >}}

Aligning Horizontal And Vetical Resolutions

This article demonstrates the usage of Aspose.Imaging for .NET to make sure that the horizontal & vetical resolutions of an image are equal while manipulating its properties. Aspose.Imaging API have exposed efficient & easy to use methods to achieve this goal. Aspose.Imaging for .NET has exposed the **AlignResolutions** method of the **Image** class for making horizontal & vertical alignment equal. The following code snippet shows you how to use **AlignResolutions** method.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "aligning-horizontal-and-vertical-resolutions-of-image.cs" >}}
## **Apply Correction Filter On An Image**
This article demonstrates the usage of Aspose.Imaging for .NET to perform correction filters on an image. Aspose.Imaging APIs have exposed efficient & easy to use methods to achieve this goal. Aspose.Imaging for .NET has exposed the **BilateralSmoothingFilterOptions** and **SharpenFilterOptions** classes for filtration. **BilateralSmoothingFilterOptions** class needs an integer as size. The steps to perform Resize are as simple as below:

1. Load an image using the factory method Load exposed by Image class.
1. Convert the image into **RasterImage**.
1. Create an instances of **BilateralSmoothingFilterOptions** and **SharpenFilterOptions** classes.
1. Call the RasterImage.Filter method while specifying rectangle as image bounds and **BilateralSmoothingFilterOptions** class instance.
1. Call the RasterImage.Filter method while specifying rectangle as image bounds and **SharpenFilterOptions** class instance.
1. Adjust the contrast
1. Set brightness
1. Save the results.

The following code snippet shows you how to apply correction filter.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "apply-correction-filter-on-image.cs" >}}
## **Use Bradley threshold algorithm**
Image thresholding is used in graphics applications. The goal of thresholding an image is to classify pixels as either “dark” or “light”. Aspose.Imaging API allows you to use Bradley thresholding while converting images. The following code snippet shows you how to define the threshold value and then invoke the Bradley’s threshold algorithm.

{{< gist "aspose-com-gists" "c03f82411d05cb85e2fb8be924e54f0b" "bradley-threshold.cs" >}}




