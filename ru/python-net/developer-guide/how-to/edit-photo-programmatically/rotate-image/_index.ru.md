---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/edit-photo-programmatically/rotate-image
linktitle: How to rotate an image
title: How to rotate an image
description: Rotate an image to a fixed angle. Flip images vertically or horizontally. Rotate photos to a selected angle.
keywords: [rotate an image, rotating image, flip an image]
---

## How to rotate an image

### Rotate and flip an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can rotate an image to a fixed angle of 90/180/270-degree with or without a flip. Use <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#rotate_flip_rotate_flip_type_83">RotateFlip method</a> and specify `ROTATE_270_FLIP_NONE` type parameter to flip on 270 degrees without flip. Python code example:
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "rotate-image.py" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Full list with all available rotate types you can find in the <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype/">Rotate and flip types parameters</a> descriptions.
</p>

### Rotate an image to the arbitrary angle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
If you want to rotate an image to arbitrary choice angle, you can use the rotate method with specific rotation angle. The angle value can be positive if a rotation is clockwise or negative for the opposite direction. The size of the original image might be changed after rotating the image, so you have to specify `Resize proportionally` boolean parameter to indicate should the resulting image resized proportionally or not. In case you want to preserve the image size after rotating, you need to specify the background color to fill the empty corners of the rotated image.
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "rotate-image-on-specific-angle.py" >}}
