---
title: How to crop an image with Aspose.Imaging program library
description: Crop an image. Select rectangle area for cropping. Crop photo by shifts.
keywords: [crop an image, image crop, crop photo, image cropping]
---

# How to crop an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can select between two types of possible cropping: either indicate new image boundaries by shifts from the sides of the image, i.e. 10 px for left, right top and bottom shifts or create a rectangle with the desired size and use it for image cropping. 
</p>

## Crop by shifts

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The example below makes an image <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/crop/#rasterimagecrop-method-2-of-2">Crop by shifts</a> on 10px from each image side:
</p>

{% gist aspose-com-gists/7ee37a401e37790396ad9f4cde87d446 cropping-by-shifts.cs %}


## Crop by rectangle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this example, we create a square with a side length of 20 px and then <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/crop/#rasterimagecrop-method-1-of-2">Crop by rectangle</a> the photo to this area from the original picture.
</p>

{% gist aspose-com-gists/7ee37a401e37790396ad9f4cde87d446 cropping-by-rectangle.cs %}
