---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/dither-image
linktitle: How to dither an image
title: How to dither an image
description: Dither an image. Dithering image with a threshold. Floyd Steinberg Dithering.
keywords: [edit an image, dither an image, dithering method, Floyd Steinberg Dithering]
---

## How to dither an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To edit an image with 
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#dither-int-int-">Dithering method</a> you can specify `ThresholdDithering` or `FloydSteinbergDithering` options.
The `ThresholdDitherig` is a simple and fast dithering method, and the `FloydSteinbergDithering` is a more complex method that takes into account nearest neighbors' pixels' intensity values. And as a second parameter, you can indicate the color palette in bits for use for dithering. More bits mean a higher quality of the resulting image, but at the same time a larger image size:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-DitheringRasterImages-DitheringRasterImages.java" >}}
