---
title: Alpha Blending Image Filter
type: docs
weight: 50
url: /java/developer-guide/manipulating-images/image-and-photo-filters/alpha-blending-image-filter/
description: Alpha blending image filter application for image overlay with opacity level settings with Java code example.
keywords: [photo filter, image filter, image effect, overlay image, alpha blending, blend image, blend method, background image, overlay alpha, overlay layer, transparency level, opacity level]
---

## Alpha Blending Image Filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This Java code example below shows the application of an alpha blending photo filter and the positioning of an overlay image onto a background image using the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#blend-com.aspose.imaging.Point-com.aspose.imaging.RasterImage-com.aspose.imaging.Rectangle-byte-">Blend method</a> of the `RasterImage` class from the Aspose.Imaging library. This method enables the control of overlay image opacity through an overlay alpha value within a range of 0 to 255. A value of 255 indicates that the overlay image is fully opaque, while a value of 0 implies complete transparency. For our example, we will utilize a semi-transparent image effect with an overlay alpha value of 127. The placement of the overlay image will be at the center of the background image, calculated as half of the background's width and height.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Once the overlay and background images are loaded, you can apply the `Blend` image filter to the background image and subsequently save the resulting image. This output image will consist of the semi-transparent overlay image positioned at the center of the background image.
</p>

{{< gist "aspose-com-gists" "ec0f58e33fbb2678ecd3c0fd2f9a0eb2" "alpha-blending.java" >}}
