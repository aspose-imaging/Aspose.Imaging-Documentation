---
title: Kernel Filters
type: docs
weight: 55
url: /python-net/developer-guide/manipulating-images/kernel-filters/
description: Aspose.Imaging graphic library for Python supports kernel filters.
keywords: [photo filter, image filter, photo effect]
---

## Kernel Filters



Identical:
```pyhton
[
    [ 0, 0, 0,],
    [ 0, 1, 0,],
    [ 0, 0, 0,],
]
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
</style>

<figure class="frame"><p>
    <img class="marginauto" src="./template-vector-svg.webp" alt="Original svg vector drawing before kernel filter" width="793" height="1123"/>
<figcaption>Original vector image</figcaption>
</p></figure>

Edge detection  custom kernel filter:
```python
[
    [ -1, -1, -1,],
    [ -1,  8, -1,],
    [ -1, -1, -1,],
]
```

<figure class="frame"><p>
    <img class="marginauto" src="./edge-dection-kernel-filter-svg.webp" alt="Edge detection 3x3 kernel filter" width="793" height="1123"/>
<figcaption>Edge detection kernel filter</figcaption>
</p></figure>

Inverse deconvolution custom kernel filter:

<figure class="frame"><p>
    <img class="marginauto" src="./deconvolution-custom-kernel-filter-svg.webp" alt="Deconvolution custom kernel filter" width="793" height="1123"/>
<figcaption>Deconvolution custom kernel filter</figcaption>
</p></figure>
