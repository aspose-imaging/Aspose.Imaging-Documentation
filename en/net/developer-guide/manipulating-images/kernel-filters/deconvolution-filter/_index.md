---
title: Deconvolution Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/deconvolution-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Convolution, Deconvolution as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, deconvolution filter, kernel matrix, convolution operation, custom kernel filter]
---

## Deconvolution Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Deconvolution serves as the inverse matrix operation to a convolution filter. If a convolution transformation is applied, such as with the <a href="../gaussian-blur-filter/">Gaussian blur kernel filter</a>, attempting to reverse this operation cannot fully restore the original image due to the averaging of pixel values and the loss of some details. However, deconvolution is valuable for image restoration and deblurring.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the example below we apply the Gaussian blur convolution filter and then restore the original image with Deconvolution filer:
</p>

```cs
// gaussian 3x3 convolution kernel
{
  {1, 2, 1,},
  {2, 4, 2,},
  {1, 2, 1,},
};
```

```cs
DeconvolutionFilterOptions(ConvolutionFilter.GetGaussian(Size, Sigma))
```
<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The restored image is not identical to the original, but it exhibits more details after the deblurring process.
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
        <figcaption>Deconvolution filter</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-landscape.webp" alt="Original landscape image" width="640" height="400"/>
    </div>
    <div>
        <img src="./deconvolution-gaussian-blur-kernel-filter.webp" alt="Deconvolution Gaussian blur kernel filter" width="640" height="400"/>
    </div>
</div>
<figcaption>Deconvolution kernel filter</figcaption>
</figure>

## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The full C# code example below shows the usage of the Aspose.Imaging .NET API. You can utilize the `ConvolutionFilter` class with "GetGaussian" blurring method and subsequently deblur using the <strong>DeconvolutionFilterOptions</strong>. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
