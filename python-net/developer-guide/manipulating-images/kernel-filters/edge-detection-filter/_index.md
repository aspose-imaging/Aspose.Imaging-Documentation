---
title: Edge Detection Filters
type: docs
weight: 55
url: /python-net/developer-guide/manipulating-images/kernel-filters/edge-detection-filter/
description: Aspose.Imaging graphic library for Python supports kernel filters such as Edge Detection, as well as custom kernels.
keywords: [photo filter Python, image filter Python, photo effect Python, kernel filter, edge detection filter, kernel matrix, convolution operation, custom kernel filter]
---

## Edge Detection Custom Kernel Filter in Python

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Crafting a custom kernel filter for edge detection echoes the characteristics of the <a href="../sharpen-filter/">Sharpen filter</a>, albeit with a distinctive point: the sum of matrix elements totals zero. Consequently, the resulting image takes on an almost entirely black appearance, punctuated only by pixels deviating from their surroundings. These exceptional pixels typically mark the boundaries between diverse areas or edges.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this illustrative scenario, the central pixel's value is compared to its neighboring pixels. You have the flexibility to define a custom kernel, finely tuned to identify edges either horizontally, vertically or both.
</p>

```python
# edge detection custom kernel
[
    [  0, -1,  0,],
    [ -1,  4, -1,],
    [  0, -1,  0,],
]
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the end, the application of the filter culminates in preserving only the contours of the image set on a black background.
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
        <figcaption>Edge detection</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="../template-vector-svg.webp" alt="Original vector image" width="793"/>
    </div>
    <div>
        <img src="./edge-detection-kernel-filter-svg.webp" alt="Edge detection 3x3 custom kernel filter in Python" width="793" />
    </div>
</div>
<figcaption>Edge detection kernel filter</figcaption>
</figure>

## Python code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The provided Python code example showcases the utilization of the Aspose.Imaging Python API. Utilize the `ConvolutionFilter` class, which provides pre-defined kernel filters, alongside the option to incorporate a `<strong>custom_kernel</strong>` matrix. In this instance, image templates in raster PNG and as well as vector SVG formats are loaded from the "templates" folder, and a range of filters are applied from a predefined list.
</p>

{{< gist "aspose-com-gists" "ff91f0a36b9bf6eae152d95791eb3bcc" "kernel-filters.py" >}}
