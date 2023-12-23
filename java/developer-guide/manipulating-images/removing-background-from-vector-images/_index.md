---
title: Remove background from vector images in Java
linktitle: Remove background from vector images
type: docs
weight: 15
url: /java/removing-background-from-vector-images/
description: Using Aspose.Imaging for Java for background removal from vector images.
keywords: Java library for background removal, remove background in Java, remove background from vector images, remove background from ODG, remove background Java example
---

## Java API for Background Removal in Vector Images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Background removal is a popular task not confined to raster images but extends to vector images as well. Aspose.Imaging for Java empowers you to seamlessly execute background removal for vector images like ODG or SVG, preserving the results in the same image format or converting them into other formats, including raster images.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Handling vector images diverges from raster formats. A background in vector files might contain multiple color objects enveloping the entire image, overlapping with foreground objects. The Aspose.Imaging identifies objects without underlying shapes as a background. Moreover, you can designate a background color for removal, excluding foreground objects of the same color from the removal process. Furthermore, you can select a particular rectangle area of the image for background removal. The eliminated background can be substituted with another color or saved with a transparent layer.
</p>

### ODG vector image example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Consider the OpenDocument Graphics (ODG) vector image example below, featuring a blue background with a hatch. The original blue background was removed and the resulting image has a transparent hatch:
</p>

<style>
   .frame {
    border: 2px solid darkgray;
    padding: 5px;
    margin: 10px 0 5px 5px;
    background: #f0f0f0;
    align-items: center;
   }
   .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
   }
    .frame figcaption {
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: center;
   }
</style>

<figure class="frame">
<div class="container">
    <div>
        <figcaption>Original image</figcaption>
    </div>
    <div>
        <figcaption>Resulting image</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="./hatch-with-background.odg.webp" alt="Vector ODG image with background" width="640" height="905"/>
    </div>
    <div>
        <img src="./hatch-removed-background.odg.webp" alt="Removed background from ODG vector image" width="640" height="905"/>
    </div>
</div>
<figcaption>Removing background from ODG vector image</figcaption>
</figure>

### Java code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Below is a Java code snippet illustrating the image processing for background removal. Automating this process for vector images involves listing all desired source file names and specifying the special settings for each one. Subsequently, we apply the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/vectorimage/#removeBackground-com.aspose.imaging.RemoveBackgroundSettings-">removeBackground() method</a> to remove the background from the vector images and rasterize images to PNG format with a transparent alpha channel.
</p>

{{< gist "aspose-com-gists" "26a3ef7a80fab1d53054422a388087a2" "remove-change-background-for-vector-images.java" >}}
