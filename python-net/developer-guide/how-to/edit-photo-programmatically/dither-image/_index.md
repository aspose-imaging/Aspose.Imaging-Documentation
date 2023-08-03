---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/dither-image
linktitle: How to dither an image
title: How to dither an image
description: Dither an image. Dithering image with a threshold. Floyd Steinberg Dithering.
keywords: [edit an image, dither an image, dithering method, Floyd Steinberg Dithering]
---

## How to dither an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To edit an image with <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/ditheringmethod/">Dithering method</a> you can specify `ThresholdDithering` or `FloydSteinbergDithering` options.
The `ThresholdDitherig` is a simple and fast dithering method, and the `FloydSteinbergDithering` is a more complex method that takes into account nearest neighbors' pixels' intensity values. And as a second parameter, you can indicate the color palette in bits for use for dithering. More bits mean a higher quality of the resulting image, but at the same time a larger image size:
</p>

{{< gist "aspose-com-gists" "95e4108a2bc8cf2db6673c1225d3123a" "dither-images.cs" >}}
