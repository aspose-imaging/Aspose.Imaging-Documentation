---
title: Kernel Filters
type: docs
weight: 55
url: /java/developer-guide/manipulating-images/kernel-filters/
description: Aspose.Imaging graphic library for Java supports kernel filters.
keywords: [photo filter, image filter, photo effect]
---

## Kernel Filters



Identical:
```java
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
    <img class="marginauto" src="./template-building.webp" alt="Original building photo before kernel filter" width="640" height="480"/>
<figcaption>Original building photo</figcaption>
</p></figure>

Sharpen 3x3:
```java
{
    {  0, -1,  0 },
    { -1,  5, -1 },
    {  0, -1,  0 },
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./sharpen3x3-kernel-filter.webp" alt="Sharpen 3x3 kernel filter" width="640" height="480"/>
<figcaption>Sharpen kernel filter</figcaption>
</p></figure>


Edge detection:
```java
// vertical edge detection
{
    { 0,  0,  0,  0,  0,},
    { 0,  0,  0,  0,  0,},
    { -1, -1, 4, -1, -1,},
    { 0,  0,  0,  0,  0,},
    { 0,  0,  0,  0,  0,},
};
```


<figure class="frame"><p>
    <img class="marginauto" src="./vertical-edge-kernel-filter.webp" alt="Vertical edges 5x5 kernel filter detection" width="640" height="480"/>
<figcaption>Vertical edges kernel filter</figcaption>
</p></figure>

```java
// horizontal edge detection
{
    { 0, 0, -1, 0, 0,},
    { 0, 0, -1, 0, 0,},
    { 0, 0,  4, 0, 0,},
    { 0, 0, -1, 0, 0,},
    { 0, 0, -1, 0, 0,},
};
```

<figure class="frame"><p>
    <img class="marginauto" src="./horizontal-edge-kernel-filter.webp" alt="Horizontal edges 5x5 kernel filter detection" width="640" height="480"/>
<figcaption>Horizontal edges kernel filter</figcaption>
</p></figure>
