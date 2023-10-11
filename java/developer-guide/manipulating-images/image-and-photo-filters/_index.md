---
title: Image and Photo Filters
type: docs
weight: 50
url: /java/developer-guide/manipulating-images/image-and-photo-filters/
description: Implementing image or photo effects for Java. Alpha blending image filter for creating watermark images with transparent overlay image logo. Magic Wand tool for color selection.
keywords: [photo filter, image filter, photo effect, overlay image, alpha blending, image effect, blend image, image manipulation, opacity levels, magic wand, color selection]
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
Increasing awareness and, consequently, web page traffic is the goal of any website owner. One effective method to attract users is by utilizing the alpha blending image filter to apply watermarks using an overlay image. Distributing images with your brand name across the internet not only increases your recognition but also safeguards the image's quality. This blend image filter serves as both advertisement and protection against image theft.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample.webp" alt="Original image" width="640" height="497"/>
    </div>
    <div>
        <img src="./images/blended_out.webp" alt="Alpha blending filter with logo overlay" width="640" height="497"/>
    </div>
</div>
<figcaption>Alpha blending image filter with logo overlay</figcaption>
</figure>

Example Java code: [alpha blending](alpha-blending-image-filter)

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
However, this isn't the only reason to include the alpha blending image effect in your arsenal of image manipulation tools. Using this image filter presents an excellent opportunity to introduce creativity into your work. For instance, you can achieve transparency effects by layering images with different opacity levels, transforming an ordinary portrait into a unique collage-like creation, and much more.
</p>


## Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The process of image editing resembles the work of an artist, but instead of a physical canvas and brushes, a designer's toolkit includes various functions, one of which is the Magic Wand tool. It proves invaluable when dealing with areas of similar color tints. With the Magic Wand tool, you can effortlessly highlight the tone you wish to adjust, and the tool will automatically select the desired areas.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample_magic_wand_blue.webp" alt="Magic Wand original image " width="600" height="400"/>
    </div>
    <div>
        <img src="./images/sample_magic_wand_java.webp" alt="Magic Wand tool blue shape color selection" width="600" height="400"/>
    </div>
</div>
<figcaption>Magic Wand tool: blue shape color selection</figcaption>
</figure>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
When editing a landscape where a vast portion of the canvas is filled with blue sky, the task may involve replacing specific tones with others. Magic Wand tool offers an option to fine-tune the degree of color tolerance. Besides its color-related capabilities, the tool excels in selecting complex masks. Smoothing the edges ensures that the final image with the object appears more natural.
</p>

<figure class="frame">
<div class="container"><div>Source image</div><div>Resulting image</div></div>
<div class="container">
    <div>
        <img src="./images/sample_mountains.webp" alt="Magic wand original image " width="640" height="425"/>
    </div>
    <div>
        <img src="./images/magic_wand_java.webp" alt="Magic wand tool blue sky color selection" width="640" height="425"/>
    </div>
</div>
<figcaption>Magic Wand tool: blue sky color selection</figcaption>
</figure>

Example Java code: [magic wand](magic-wand-filter/)

## Remove watermark

Example Java code: [remove watermark](remove-watermark-filter/)
