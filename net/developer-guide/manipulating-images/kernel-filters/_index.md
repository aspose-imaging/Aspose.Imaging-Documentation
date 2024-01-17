---
title: Kernel Filters
type: docs
weight: 55
url: /net/developer-guide/manipulating-images/kernel-filters/
description: Aspose.Imaging graphic library for .NET (C#) supports kernel filters.
keywords: [photo filter, image filter, photo effect]
---

## Kernel Filters



Identical:
```cs
{
    { 0, 0, 0,},
    { 0, 1, 0,},
    { 0, 0, 0,},
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
</style>

<figure class="frame"><p>
    <img class="marginauto" src="./template-landscape.webp" alt="Original photo template before kernel filter" width="640" height="400"/>
<figcaption>Original photo template</figcaption>
</p></figure>

Emboss 3x3:
```cs
{
    { -2, -1,  0, },
    { -1,  1,  1, },
    {  0,  1,  2, },
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./emboss3x3-kernel-filter.webp" alt="Emboss 3x3 kernel filter" width="640" height="400"/>
<figcaption>Emboss 3x3 kernel filter</figcaption>
</p></figure>

Sharpen 3x3:
```cs
{
    {  0, -1,  0 },
    { -1,  5, -1 },
    {  0, -1,  0 },
};
```

BlurBox 5x5:
```cs
{
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
    { 0.04, 0.04, 0.04, 0.04, 0.04,},
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./blur-box-5x5-kernel-filter.webp" alt="Blur Box 5x5 kernel filter" width="640" height="400"/>
<figcaption>BlurBox kernel filter</figcaption>
</p></figure>


Custom kernel matrix for MotionBlur 5x5 45%:
```cs
double[,] customKernel = new double[,]
{
  { 0.25, 0,   0,   0,   0    },
  { 0,    0.2, 0,   0,   0    },
  { 0,    0,   0.1, 0,   0    },
  { 0,    0,   0,   0.2, 0    },
  { 0,    0,   0,    0,  0.25 },
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./custom-motion-blur-kernel-filter.webp" alt="Custom Motion blur 5x5 45% kernel filter" width="640" height="400"/>
<figcaption>Custom Motion blur kernel filter</figcaption>
</p></figure>
