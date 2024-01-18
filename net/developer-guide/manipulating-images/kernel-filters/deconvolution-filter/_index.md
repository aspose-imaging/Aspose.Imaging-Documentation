---
title: Deconvolution Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/deconvolution-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Convolution, Deconvolution as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, deconvolution filter, kernel matrix, convolution operation, custom kernel filter]
---

## Deconvolution Filter

```cs
// gaussian convolution kernel
{
  {1, 2, 1,},
  {2, 4, 2,},
  {1, 2, 1,},
};
```

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
The following C# code example illustrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters such as "Emboss3x3," "GetBlurBox" with customizable size settings, "GetBlurMotion" with adjustable size and angle settings. Additionally, you have the flexibility to create your custom kernel matrix. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
