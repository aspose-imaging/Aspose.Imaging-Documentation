---
title: Alpha Blending Image Filter
type: docs
weight: 50
url: /ru/python-net/developer-guide/manipulating-images/image-and-photo-filters/alpha-blending-image-filter/
description: Alpha blending image and photo filter for Python. The alpha blending provides an image effect of the overlay image placed on the transparency layer above a background image.
keywords: [photo filter, image filter, image effect, overlay image, alpha blending, blend image, blend method, background image, overlay alpha, overlay layer, transparency level, opacity level]
---

## Alpha Blending Image Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging library provides the <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#blend_origin_overlay_overlay_area_overlay_alpha_9">Blend method</a> to achieve alpha blending image or photo effect. Using this image filter on a background creates the image effect of placing the overlay image over a transparent layer on top of the background. The `Blend` method allows you to specify the coordinates of the point on the background where you want to place the overlay image. Overlay images can be inserted with varying levels of opacity, ranging from 0 (fully transparent) to 255 (fully opaque), known as the "overlay alpha" value.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the Python example provided below, we show a semi-transparent overlay image with an opacity level of 127 placed in the center of a background image. The resulting image is then saved to an output file.
</p>

{{< gist "aspose-com-gists" "afd9bfb6106e0734c36dfa251094bad9" "alpha-blending.py" >}}
