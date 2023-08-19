---
title: Image and Photo Filters
type: docs
weight: 50
url: /net/developer-guide/manipulating-images/image-and-photo-filters/
description: Alpha blending image filter application for placing semi-transparent images on top of a background image.
keywords: [photo filter, image filter, photo effect, image overlay, alpha blending, image effect, blend image, watermarking images]
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
Despite the vast possibilities offered by modern computer graphics, it's becoming progressively challenging to captivate users in the online realm. However, images that exhibit not only mastery but also ingenuity have the potential to generate maximum traffic to a webpage. For instance, achieving a misty photo effect in a landscape doesn't necessitate acquiring paints; employing alpha blending image filter is sufficient.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Beyond artistic applications, alpha blending image filter serves a crucial role in watermarking images. Through alpha blending, you can not only establish the author's ownership but also promote the identity of an individual or a company. In the image example below, we've positioned a semi-transparent Aspose logo onto the original document.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample.webp" alt="Original image without watermark" width="640" height="497"/>
    </div>
    <div>
        <img src="./images/blended_out.webp" alt="Alpha blending filter with logo overlay" width="640" height="497"/>
    </div>
</div>
<figcaption>Alpha blending image filter with logo overlay image</figcaption>
</figure>

Example C# code: [alpha blending](alpha-blending-image-filter)
