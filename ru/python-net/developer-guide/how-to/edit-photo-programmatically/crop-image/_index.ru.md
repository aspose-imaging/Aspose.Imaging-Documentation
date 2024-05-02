---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/edit-photo-programmatically/crop-image
linktitle: How to crop an image
title: How to crop an image
description: Crop an image. Select a rectangle area for cropping. Crop photo by shifts.
keywords: [crop an image, image crop, crop photo, image cropping]
---

## How to crop an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To crop an image you can select between two cropping types: either indicate new image boundaries by shifts from the sides of the image, i.e. 10 px for left, right, top and bottom sides or select a rectangle with the appropriate sizes and use it for image cropping.
</p>

### Crop by shifts

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The example below crop an image by utilizing the <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#crop_left_shift_right_shift_top_shift_bottom_shift_21">crop by shift method</a> with size of 10px from each image side:
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "cropping-by-shifts.py" >}}


### Crop by rectangle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this example, we create a square with a side length of 20 px and then crop an image using <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#crop_rectangle_22">crop by rectangle method</a> applied this area to the original photo:
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "cropping-by-rectangle.py" >}}
