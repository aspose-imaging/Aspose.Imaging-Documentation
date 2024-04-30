---
title: Gaussian Blur Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/gaussian-blur-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Gaussian Blur as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, blur image, blur filter, Gaussian blur, kernel matrix, convolution operation, custom kernel filter]
---

## Gaussian Blur Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 Unlike common <a href="../blur-filter/">BlurBox image filters</a> using a box or averaging filter, applies a simple average to the pixel values in a defined neighborhood. This results in a uniform and straightforward blurring effect, where each pixel contributes equally to its neighbors. On the other hand, Gaussian blur employs a Gaussian distribution to determine the weights of pixels in the neighborhood. This means that pixels closer to the center have higher weights, creating a smoother and more natural blurring effect. To emulate the Gaussian distribution, the following 3x3 matrix can be used:
</p>

```cs
// gaussian blur 3x3 kernel
{
  {1, 2, 1,},
  {2, 4, 2,},
  {1, 2, 1,},
};
```
<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To preserve the luminosity of the source image, all elements are divided by 16, which represents the sum of the matrix elements.
</p>

```cs
// gaussian blur 3x3 kernel /16
double[,] customKernel = new double[,]
{
  { 0.0625, 0.125,  0.0625,},
  { 0.125,   0.25,   0.125,},
  { 0.0625, 0.125,  0.0625,},
};
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Gaussian blur tends to produce a more visually appealing and realistic result compared to the uniform blurring of common blur filters.
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
   .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
   }
</style>

<figure class="frame">
<div class="container">
    <div>
        <figcaption>Original image</figcaption>
    </div>
    <div>
        <figcaption>Gaussian blur</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-landscape.webp" alt="Original landscape image" width="640" height="400"/>
    </div>
    <div>
        <img src="./gaussian-blur-kernel-filter.webp" alt="Gaussian blur kernel filter" width="640" height="400"/>
    </div>
</div>
<figcaption>Gaussian blur kernel filter</figcaption>
</figure>


## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The following C# code example illustrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters such as <strong>GetGaussian()</strong> method with adjustable size and sigma value of Gauss distribution. Additionally, you have the flexibility to create your custom kernel matrix. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
