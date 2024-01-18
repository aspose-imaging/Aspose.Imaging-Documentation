---
title: Kernel Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Emboss, Blur, MotionBlur as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, blur image, emboss image, motion blur filter, kernel matrix, convolution operation, blurbox filter, gaussian blur, custom kernel filter]
---

## Kernel Filters for Image Processing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Kernel filters serve as a powerful tool for image processing, enabling the creation of a wide range of image effects, such as `Emboss`, `Blur`, `MotionBlur`, `GaussianBlur` and others. Aspose.Imaging for .NET not only supports standard kernel filters but also provides the flexibility to create custom filters and empower the development of unique image and photo effects. These filters leverage a matrix known as a "kernel," describing the pixel manipulations required on the source image bitmap to achieve the intended effect. The filter algorithm consequently applies the kernel matrix to each pixel of the source image, using a matrix operation similar to a mathematical convolution operation.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Consider a simple matrix with dimensions 3x3, populated with zeros except for the central element set to 1. It is crucial for the kernel matrix to consistently have even dimensions, ensuring the presence of a central point:
</p>

```cs
// identical kernel
{
    { 0, 0, 0,},
    { 0, 1, 0,},
    { 0, 0, 0,},
};
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The central element serves as the multiplication coefficient applied to the consequently selected pixel of the source image. In this scenario, multiplying the source pixel values (comprising RGB color components) by 1 results in the same value. Surrounding elements are sequentially applied to the pixels around the central pixel, and the resulting pixel values are the sum of these multiplications. In this specific case, multiplication by zero yields zero, rendering the pixels around the central element not contributing to the outcome. Therefore, our simple kernel filter produces an image identical to the original one.
</p>

<style>
   .frame {
    border: 2px solid darkgray;
    padding: 5px;
    margin: 10px 0 5px 5px;
    background: #f0f0f0;
    align-items: center;
   }
   .marginauto {
    margin: 10px auto 20px;
    display: block;
   }
   .frame figcaption {
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: center;
   }
</style>

<figure class="frame"><p>
    <img class="marginauto" src="./template-landscape.webp" alt="Original photo template before kernel filter" width="640" height="400"/>
<figcaption>Original photo template</figcaption>
</p></figure>

### BlurBox Filter

### Deconvolution Filter

### Edge Detection Filter

### Emboss Filter

### Gaussian Blur Filter

### Motion Blur Filter

### Sharpen Filter


<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This article showcases how to utilize the Aspose.Imaging .NET API for various image effects using both predefined and custom kernel filters. You can install Aspose.Imaging library from <a href="https://www.nuget.org/packages/Aspose.Imaging/">NuGet Packet Manager</a>.
</p>
