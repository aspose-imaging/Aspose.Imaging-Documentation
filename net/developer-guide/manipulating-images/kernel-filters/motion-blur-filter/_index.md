---
title: Motion Blur Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/motion-blur-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such MotionBlur as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, blur image, MotionBlur filter, kernel matrix, convolution operation, custom kernel filter]
---

## Motion Blur Custom Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You have the option to design a custom kernel with elements positioned, for instance, exclusively along one diagonal. In such a scenario, the pixel value is determined by the weighted mean of these pixels, producing the 'Motion Blur' image effect. This effect simulates the appearance of camera movement during photo capture in a diagonal direction.
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
        <figcaption>MotionBlur filter</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-landscape.webp" alt="Original photo before emboss filter" width="640" height="400"/>
    </div>
    <div>
        <img src="./custom-motion-blur-kernel-filter.webp" alt="Custom Motion blur 5x5 45grad kernel filter" width="640" height="400"/>
    </div>
</div>
<figcaption>Custom MotionBlur kernel filter</figcaption>
</figure>


## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The following C# code example illustrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters such as "Emboss3x3," "GetBlurBox" with customizable size settings, "GetBlurMotion" with adjustable size and angle settings. Additionally, you have the flexibility to create your custom kernel matrix. In this example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
