---
title: Gaussian Blur Filters
type: docs
weight: 55
url: /python-net/developer-guide/manipulating-images/kernel-filters/gaussian-blur-filter/
description: Aspose.Imaging graphic library for Python supports kernel filters such Gaussian Blur as well as custom kernels.
keywords: [photo filter Python, image filter Python, photo effect Python, kernel filter, blur image, blur filter, Gaussian blur, kernel matrix, convolution operation, custom kernel filter]
---

## Gaussian Blur Kernel Filter in Python

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The <a href="../blur-filter/">Blur Box image filters</a> use pixel values averaging based on a uniform distribution, the alternative approach employs a pixel-wise average within a specified neighborhood. In contrast to a Blur Box, the Gaussian blur leverages a Gaussian distribution, intricately assigning weights to pixels based on their proximity to the center. This results in a more refined and natural blurring effect, as pixels nearer to the center carry higher weights. The following 5x5 matrix can be used for the Gaussian approximation:
</p>

```python
# gaussian blur 5x5 kernel
[
 [1, 4,  6,  4,  1],
 [4, 16, 24, 16, 4],
 [6, 24, 36, 24, 6],
 [4, 16, 24, 16, 4],
 [1, 4,  6,  4,  1],
]
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To maintain the luminosity of the source image, it is imperative to divide all elements by 256, representing the sum of the matrix elements.

Gaussian blur, in contrast to the uniform blurring observed in typical blur filters, tends to yield a visually more appealing and realistic result.
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
        <img src="../template-vector-svg.webp" alt="Original vector image" width="793" />
    </div>
    <div>
        <img src="./gaussian-blur-kernel-filter.svg.webp" alt="Gaussian blur 5x5 kernel filter in Python" width="793" />
    </div>
</div>
<figcaption>Gaussian blur kernel filter</figcaption>
</figure>


## Python code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The provided Python code example serves as an illustration of the Aspose.Imaging Python API's usage. Utilize the `ConvolutionFilter` class, which provides pre-defined kernel filters, including the <strong>get_gaussian()</strong> method with customizable size and sigma values for Gaussian distribution. Moreover, you retain the flexibility to craft your personalized kernel matrix. Within this example, image templates in raster PNG and as well as vector SVG formats are loaded from the "templates" folder, and a set of filters are applied from the `kernel_filters` list.
</p>

{{< gist "aspose-com-gists" "ff91f0a36b9bf6eae152d95791eb3bcc" "kernel-filters.py" >}}
