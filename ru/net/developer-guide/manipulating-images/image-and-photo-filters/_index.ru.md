---
title: Image and Photo Filters
type: docs
weight: 50
url: /ru/net/developer-guide/manipulating-images/image-and-photo-filters/
description: Aspose.Imaging graphic library for .NET (C#) supports Alpha blending image filter for placing semi-transparent images on top of a background image. Magic Wand tool for color area selection. Watermark removal filter automatically fills the marked area with similar image fragments.
keywords: [photo filter, image filter, photo effect, image overlay, alpha blending, image effect, blend image, watermarking images, magic wand, color selection, watermark removal, remove watermark]
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


## Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Working with images and photos often involves operations such as selecting a specific color area to adjust or replace with another. Without a tool like the Magic Wand, graphic designers would face extreme difficulty in selecting areas with complex outlines or multiple areas sharing a similar color. With the Magic Wand, you can simply choice on a point within a single-color area, and the tool will automatically select the entire area around it that shares a similar color. 
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample_magic_wand_light_blue.webp" alt="Original image before magic wand" width="600" height="400"/>
    </div>
    <div>
        <img src="./images/sample_magic_wand_net.webp" alt="Magic wand tool light-blue color selection" width="600" height="400"/>
    </div>
</div>
<figcaption>Magic Wand tool: light-blue color selection</figcaption>
</figure>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can adjust the degree of color similarity by setting a threshold for color comparison. The areas selected using this method can be combined, subtracted from one another, or have the selection inverted. Feathering can also be applied to the edges of the areas to achieve a smooth transition. In the example shown in the image below, we selected the green background area around the shape, added yellow specks to the selection, and then removed the resulting mask from the original image. As a result, we will obtain a figure without a background, which can then be used for creating other graphic works.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample_magic_wand_tool.webp" alt="Original image before magic wand" width="640" height="360"/>
    </div>
    <div>
        <img src="./images/magic_wand_tool.webp" alt="Magic wand tool green background color selection" width="640" height="360"/>
    </div>
</div>
<figcaption>Magic Wand tool: green background color selection</figcaption>
</figure>

Example C# code: [magic wand](magic-wand-filter/)

## Remove watermark image filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Certain smartphones and cameras can add watermarks to photos as they capture them. These watermarks can include manufacturer logos or device model names. If you need to share these photos without these unwanted marks, you can use the Watermark Removal image filter.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To effectively remove these watermarks, you need to define the area where the mark is located by indicating its coordinates. Utilizing the available image data, the algorithm will automatically replace the watermark area with similar fragments. In the image filter options, you can choose between the `Content-Aware Fill` or the `Telea` watermark removal algorithm. Furthermore, you can specify the number of attempts to remove the watermark. In this scenario, the algorithm will determine the best result.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/landscape_watermark.webp" alt="Original image before removal" width="640" height="360"/>
    </div>
    <div>
        <img src="./images/landscape_watermark_removed.webp" alt="Image after watemark removal" width="640" height="360"/>
    </div>
</div>
<figcaption>Watermark removal filter example</figcaption>
</figure>

Example C# code: [remove watermark](remove-watermark-filter/)
