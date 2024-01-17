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


### Identical Image Filter

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


### Emboss Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this example, we manipulate pixel values based on their surrounding counterparts. The resulting pixel values are proportionally diminished relative to the values of the top-left surrounding pixels and increased in correspondence to the bottom-right corner surroundings. Essentially, brighter top-left pixels lead to a greater decrease in value, while a brighter bottom-right pixel results in an increase in value. The maximum value of 255 represents white, and 0 corresponds to black color. If the result exceeds 255, it is capped at 255, and values below 0 are adjusted to 0. The sum of all matrix coefficients remains equal to 1, ensuring that the overall brightness of the image stays constant.
</p>

```cs
// emboss3x3 kernel
{
    { -2, -1,  0, },
    { -1,  1,  1, },
    {  0,  1,  2, },
};
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Hence, the image edges and contours are visually enhanced, acquiring more shadow from the top-left side and increased light from the bottom-right side. This image effect, known as the "Emboss" filter, relates the appearance of the image being embossed or elevated from the background. The result is a visual illusion of depth and texture.
</p>

<figure class="frame"><p>
    <img class="marginauto" src="./emboss3x3-kernel-filter.webp" alt="Emboss 3x3 kernel filter" width="640" height="400"/>
<figcaption>Emboss 3x3 kernel filter</figcaption>
</p></figure>


### BlurBox Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
By populating the kernel matrix with equal elements and ensuring a total sum of 1, you can compute the mean value of the surrounding pixel area with a size of 5x5. This process effectively helps eliminate noise and results in a 'Blur Box' image effect.
</p>

```cs
// BlurBox 5x5 kernel
{
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./blur-box-5x5-kernel-filter.webp" alt="Blur Box 5x5 kernel filter" width="640" height="400"/>
<figcaption>BlurBox kernel filter</figcaption>
</p></figure>


### Motion Blur Custom Kernel

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Alternatively, you have the option to design a custom kernel with elements positioned, for instance, exclusively along one diagonal. In such a scenario, the pixel value is determined by the weighted mean of these pixels, producing the 'Motion Blur' image effect. This effect simulates the appearance of camera movement during photo capture in a diagonal direction.
</p>

```cs
// custom MotionBlur 5x5 kernel
double[,] customKernel = new double[,]
{
  { 0.25, 0,   0,   0,   0    },
  { 0,    0.2, 0,   0,   0    },
  { 0,    0,   0.1, 0,   0    },
  { 0,    0,   0,   0.2, 0    },
  { 0,    0,   0,    0,  0.25 },
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./custom-motion-blur-kernel-filter.webp" alt="Custom Motion blur 5x5 45grad kernel filter" width="640" height="400"/>
<figcaption>Custom Motion blur kernel filter</figcaption>
</p></figure>

## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The following C# code example illustrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters such as "Emboss3x3," "GetBlurBox" with customizable size settings, "GetBlurMotion" with adjustable size and angle settings. Additionally, you have the flexibility to create your custom kernel matrix. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This article showcases how to utilize the Aspose.Imaging .NET API for various image effects using both predefined and custom kernel filters. You can install Aspose.Imaging library from <a href="https://www.nuget.org/packages/Aspose.Imaging/">NuGet Packet Manager</a>.
</p>
