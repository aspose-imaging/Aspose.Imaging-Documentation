---
title: Remove background from vector images in C#
linktitle: Remove background from vector images
type: docs
weight: 15
url: /net/removing-background-from-vector-images/
description: Setting some of the pixel values in an image to zero, or some other “background” value is known as Masking. C# Image Processing Library supports the following types of masking.
keywords: remove background from vector images, remove background from EMF, remove background from SVG, remove background from WMF, remove background from CDR
---

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
        <img src="./test-with-background.odg.webp" alt="Vector ODG image with background" width="640" height="905"/>
    </div>
    <div>
        <img src="./test-removed-background.odg.webp" alt="Removed background from ODG vector image" width="640" height="905"/>
    </div>
</div>
<figcaption>Removing background from vector image</figcaption>
</figure>

C# code example:

{{< gist "aspose-com-gists" "c28d7d7f7dff39444751b5724d5ba14a" "remove-change-background-from-vector-images.cs" >}}
