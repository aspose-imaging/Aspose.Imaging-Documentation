---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/crop-image
linktitle: How to crop an image
title: How to crop an image
description: Crop an image. Select a rectangle area for cropping. Crop photo by shifts.
keywords: [crop an image, image crop, crop photo, image cropping]
---

## How to crop an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Image cropping supports two types of possible methods: either crop by defining new image boundaries by shifts from the sides of the image, for example, 10 px for left, right top and bottom shifts or to indicate a rectangle area to use for the image cropping.
</p>

### Crop by shifts

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Please see the example below which use the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#crop-int-int-int-int-">Crop method</a> of the Java class <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/">RasterImage</a> to crop the image by shifts on 10px from each side:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Jpeg-CroppingByShifts.java" >}}


### Crop by rectangle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This example shows how to create a rectangle area with a sides length of 20 px and then <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#crop-com.aspose.imaging.Rectangle-">Crop by rectangle</a> the selected area from the original picture:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Jpeg-CroppingByRectangle.java" >}}
