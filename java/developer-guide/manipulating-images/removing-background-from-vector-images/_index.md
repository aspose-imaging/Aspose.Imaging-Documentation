---
title: Remove background from vector images in Java
linktitle: Remove background from vector images
type: docs
weight: 15
url: /java/removing-background-from-vector-images/
description: Setting some of the pixel values in an image to zero, or some other “background” value is known as Masking. Java Image Processing Library supports the following types of masking.
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
        <img src="./hatch-with-background.odg.webp" alt="Vector ODG image with background" width="640" height="905"/>
    </div>
    <div>
        <img src="./hatch-removed-background.odg.webp" alt="Removed background from ODG vector image" width="640" height="905"/>
    </div>
</div>
<figcaption>Removing background from ODG vector image</figcaption>
</figure>

Java code example:

{{< gist "aspose-com-gists" "26a3ef7a80fab1d53054422a388087a2" "remove-change-background-for-vector-images.java" >}}
