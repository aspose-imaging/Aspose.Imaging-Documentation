---
title: Emboss Filters
type: docs
weight: 55
url: /ru/net/developer-guide/manipulating-images/kernel-filters/emboss-filter/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters such Emboss3x3 as well as custom kernels.
keywords: [photo filter C#, image filter C#, photo effect C#, kernel filter, emboss image, kernel matrix, convolution operation,  custom kernel filter]
---

## Emboss Kernel Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this example, we manipulate pixel values based on their surrounding counterparts. The resulting pixel values are proportionally diminished relative to the values of the top-left surrounding pixels and increased in correspondence to the bottom-right corner surroundings. Essentially, brighter top-left pixels lead to a greater decrease in value, while a brighter bottom-right pixel results in an increase in value. The maximum value of 255 represents white, and 0 corresponds to black color. If the result exceeds 255, it is capped at 255, and values below 0 are adjusted to 0. The sum of all matrix coefficients remains equal to 1, ensuring that the overall brightness of the image stays constant.
</p>

```cs
// emboss3x3 kernel
double[,] customKernel = new double[,]
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
        <figcaption>Emboss filter</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-landscape.webp" alt="Original photo before emboss filter" width="640" height="400"/>
    </div>
    <div>
        <img src="./emboss3x3-kernel-filter.webp" alt="Emboss 3x3 kernel filter" width="640" height="400"/>
    </div>
</div>
<figcaption>Emboss 3x3 kernel filter</figcaption>
</figure>


## C# code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The following C# code example demonstrates the usage of the Aspose.Imaging .NET API. You can employ the `ConvolutionFilter` class, which offers predefined kernel filters "Emboss3x3" and "Emboss5x5" with different kernel matrix sizes. Additionally, you have the flexibility to create your custom kernel matrix. In this code example, image templates in PNG and SVG formats are loaded from the "templates" folder, and filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "a1e5930122ddaf08d6960cb18782d55f" "kernel-filters.cs" >}}
