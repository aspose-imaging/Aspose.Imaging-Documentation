---
title: Remove Background from Vector Images in Python
linktitle: Remove background from vector images
type: docs
weight: 15
url: /python-net/removing-background-from-vector-images/
description: Aspose.Imaging graphic library for Python supports background removal from vector images.
keywords: remove background in Python, remove background from vector images, Windows Metafile background removal, remove background from WMF, remove background from SVG
---

## Removing Background from Vector Images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Removing backgrounds from images is a crucial task, not only for raster images but also for vector images. With the Aspose.Imaging Python API, you can seamlessly perform background removal for vector images like WMF or SVG, saving the results in the same image format or converting them to other formats, including raster images.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Processing vector images differs from raster formats. In vector files, the background may consist of multiple color-filled shapes covering the entire image, overlapping with foreground shapes or paths. In the Aspose.Imaging library, shapes without underlined paths are considered the background. Furthermore, you can specify a background color to be removed from the image and exclude foreground objects of the same color from removal. Additionally, you have the flexibility to choose a specific area of the image for background removal. The removed background can then be replaced with another color or left transparent.
</p>

### WMF vector image example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Below is an example of a Windows Metafile (WMF) vector image featuring a map drawing. The original file had its background removed, resulting in an image with a transparent background:
</p>

<style>
   .frame {
    border: 2px solid darkgray;
    padding: 5px;
    margin: 10px 0 5px 5px;
    background: #fdfdfd;
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
        <img src="./citymap-with-background.wmf.webp" alt="Vector WMF image with background" width="640" height="494"/>
    </div>
    <div>
        <img src="./citymap-removed-background.wmf.webp" alt="Removed background from WMF vector image" width="640" height="494"/>
    </div>
</div>
<figcaption>Removing background from WMF vector image</figcaption>
</figure>

### Python code example

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Python code example below demonstrates the image processing for background removal. To automate this process for vector images, you can list all the desired source file names and specify the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/removebackgroundsettings/">`RemoveBackgroundSettings`</a> for each. Then, pass these file lists and settings to the function, and utilize the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/vectorimage/#remove_background_settings_29">`removeBackground()` method</a>. The resulting images in this example are saved in the PNG raster image format with a transparent background:
</p>

{{< gist "aspose-com-gists" "291380aac991e0869dbabba3e60f5225" "remove-background-from-vector-images.py" >}}
