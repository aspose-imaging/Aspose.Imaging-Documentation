---
title: Blur Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/blur-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Blur as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, blur image, blur filter, blur box filter, kernel matrix, convolution operation, custom kernel filter]
---

## Blur Box Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
By filling the kernel matrix with uniform elements and ensuring a total sum of 1, you can determine the average value of the surrounding pixel area with a size of 5x5. The resulting pixel value is then computed as the sum of 1/25 values from all surrounding pixels. This particular kernel matrix is recognized as a 'Blur Box'. Increasing the dimensions of the matrix will intensify the blurring effect.
</p>

```cs
// Blur Box 5x5 kernel
double[,] customKernel = new double[,]
{
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
};
```
<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This process results in a gradual transition between neighboring pixel values, effectively blurring the image, helping eliminate noise, reducing sharpness and creating a smooth, vague appearance.
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
        <figcaption>Blur filter</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-landscape.webp" alt="Original photo before emboss filter" width="640" height="400"/>
    </div>
    <div>
        <img src="./blur-box-5x5-kernel-filter.webp" alt="Blur Box 5x5 kernel filter" width="640" height="400"/>
    </div>
</div>
<figcaption>Blur Box kernel filter</figcaption>
</figure>

## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The following C# code example illustrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters such as <strong>GetBlurBox()</strong> with size settings. Additionally, you have the flexibility to create your custom kernel matrix. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
