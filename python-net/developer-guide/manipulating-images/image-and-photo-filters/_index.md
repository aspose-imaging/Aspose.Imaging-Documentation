---
title: Image and Photo Filters
type: docs
weight: 50
url: /python-net/developer-guide/manipulating-images/image-and-photo-filters/
description: Creating overlay images with alpha blending image filter. Watermark image with company logo.
keywords: [image filter, photo effects, overlay images, alpha blending, image effect, blending image, watermark images]
---

<style>
   .frame {
    border: 2px solid darkgray;
    padding: 5px;
    margin: 0 auto;
    background: #f0f0f0;
    align-items: center;
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

## Alpha blending image filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Graphic work involving images can be demanding and time-consuming, especially when tasks contain overlay images. How you can effectively manage color interactions between overlapping images while maintaining varying levels of transparency? The alpha blending image filter offers a seamless solution to these challenges, streamlining your workflow and enhancing image quality. This tool proves beneficial for artists creating a visual masterpiece with photo effects as well as individuals working on scientific illustrations. High-quality images are bound to capture attention and draw more users to your webpage, particularly if you incorporate watermark images with your company logo.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample.webp" alt="Original image" width="640" height="497"/>
    </div>
    <div>
        <img src="./images/blended_out.webp" alt="Alpha blending filter with company logo overlay" width="640" height="497"/>
    </div>
</div>
<figcaption>Alpha blending image filter with logo overlay</figcaption>
</figure>

Example Python code: [alpha blending](alpha-blending-image-filter)
