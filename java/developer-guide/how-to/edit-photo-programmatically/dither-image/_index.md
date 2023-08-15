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
Image editing with 
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#dither-int-int-">Dithering method</a> requires to specify `ThresholdDithering` or `FloydSteinbergDithering` options.
The `ThresholdDitherig` option uses a simple and fast dithering method, and on the contrary, the `FloydSteinbergDithering` is a more complex method that uses the average value of nearest neighbors' pixels' intensities. The second parameter defines the color palette in bits for use for dithering. You can choose more bits for higher quality of the resulting image, but at the same time you will have a larger image file:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-DitheringRasterImages-DitheringRasterImages.java" >}}
