---
title: Alpha Blending Image Filter
type: docs
weight: 50
url: /python-net/developer-guide/manipulating-images/image-and-photo-filters/alpha-blending-image-filter/
description: Alpha blending image and photo filter for Python. The alpha blending provides an image effect of the overlay image placed on the transparency layer above a background image.
keywords: [photo filter, image filter, image effect, overlay image, alpha blending, blend image, blend method, background image, overlay alpha, overlay layer, transparency level, opacity level]
---

## Alpha Blending Image Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Aspose.Imaging library offers the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#blend_origin_overlay_overlay_area_overlay_alpha_9">Blend method</a> to implement an alpha-blending image or photo filter. Utilizing this method on a background image produces the image effect of placing an overlay image on a transparency layer above the background. By using the `Blend` method, you can specify the coordinates of the point on the background where the overlay image should be positioned. Overlay images can be inserted with varying opacity levels, ranging from 0 (fully transparent) to 255 (completely opaque), which is known as the `overlay alpha` value.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the provided Python example below, we show the placement of a semi-transparent overlay image with an opacity level of 127 at the center of the background image. The resulting image is then saved to an output file.
</p>

{{< gist "aspose-com-gists" "afd9bfb6106e0734c36dfa251094bad9" "alpha-blending.py" >}}
