---
title: Alpha Blending Image Filter
type: docs
weight: 50
url: /net/developer-guide/manipulating-images/image-and-photo-filters/alpha-blending-image-filter/
description: Alpha blending image filter application for image overlay on transparency layer above a background image. C# code example provided.
keywords: [photo filter, image filter, overlay image, alpha blending, blend image, blend method, background image, overlay alpha, overlay layer, transparency level, opacity layer]
---

## Alpha Blending Image Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The provided C# code example below demonstrates the application of an alpha blending image or photo filter. This involves loading two images: the first is the background source image or photo, and the second is the overlay image, which will be positioned on a transparent layer above the background. Both images are loaded as instances of the `RasterImage` class. Starting from Aspose.Imaging library version 23.7, the RasterImage class supports a new <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/blend/">Blend method</a>.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can utilize the `Blend` method on the background image and provide several parameters: a `Point` object indicating where to place the overlay image within the background, the overlay image object itself, the specified rectangle area of the overlay image, and an alpha value for the overlay. In this example, we calculate the coordinates to position the overlay image at the center of the background image. The overlay alpha value is set to 127, indicating a moderate level of opacity for the overlay layer. An overlay alpha value close to 0 indicates high transparency, while the maximum value of 255 indicates no transparency at all for the overlay layer.
</p>

{{< gist "aspose-com-gists" "09b74775d8be530be38f26ae5b56ad01" "alpha-blending.cs" >}}
