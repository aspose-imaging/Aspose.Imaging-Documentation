---
title: Sharpen Filters
type: docs
weight: 55
url: /python-net/developer-guide/manipulating-images/kernel-filters/sharpen-filter/
description: Aspose.Imaging graphic library for Python supports kernel filters such as Sharpen, as well as custom kernels.
keywords: [photo filter Python, image filter Python, photo effect Python, kernel filter, sharpen image, sharpen filter, kernel matrix, convolution operation, custom kernel filter]
---

## Sharpen Kernel Filter in Python

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can achieve a Sharpen image effect by establishing a kernel matrix that amplifies pixel values in comparison to their surroundings. In this instance, the central element is allocated a value five times greater than its adjacent pixels, accompanied by a subtraction for the four surrounding pixels. This configuration ensures that the cumulative sum of coefficients remains at 1, conserving the original brightness. The impact is more noticeable when neighboring pixels exhibit variations, accentuating the contrast between pixels and elevating the sharpness of the image.
</p>

```python
## sharpen 3x3 kernel
[
    [  0, -1,  0 ],
    [ -1,  5, -1 ],
    [  0, -1,  0 ],
]
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Sharpen effect improves an image by accentuating pixel contrasts, leading to enhanced image detail and better overall visual clarity.
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
        <figcaption>Sharpen image</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-vector-svg.webp" alt="Original vector image" width="793" />
    </div>
    <div>
        <img src="./sharpen-3x3-kernel-filter.svg.webp" alt="Sharpen 3x3 kernel filter in Python" width="793" />
    </div>
</div>
<figcaption>Sharpen kernel filter</figcaption>
</figure>

## Python code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The provided Python code example showcases how to utilize the Aspose.Imaging Python API. Utilize the `ConvolutionFilter` class, which provides pre-defined kernel filters like <strong>get_sharpen_3x3()</strong> and <strong>get_sharpen_5x5()</strong> methods. Moreover, you retain the freedom to craft your custom kernel matrix. In this case, image templates in raster PNG and as well as vector SVG formats are loaded from the "templates" directory, and a set of filters is applied from the `kernel_filters` list.
</p>

{{< gist "aspose-com-gists" "ff91f0a36b9bf6eae152d95791eb3bcc" "kernel-filters.py" >}}
