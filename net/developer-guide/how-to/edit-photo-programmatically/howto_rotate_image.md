---
title: How to rotate an image with Aspose.Imaging program library
description: Rotate an image to a fixed angle. Flip images vertically or horizontally. Rotate photos to a selected angle.
keywords: [rotate an image, rotating image]
---

# How to rotate an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The first type of rotating image is a rotation to a fixed angle of 90/180/270-degree with or without a flip. You just need to load your image and apply the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/image/rotateflip/">RotateFlip method</a> with a rotate type parameter. We use the type `Rotate270FlipNone` in this example:
</p>

{% gist aspose-com-gists/7ee37a401e37790396ad9f4cde87d446 rotate-image.cs %}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a full list of available types please see the link to the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rotatefliptype/">rotate and flip types parameters</a> descriptions.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The second type is rotating for an arbitrary choice angle. The rotation angle value could be positive if a rotation is clockwise or negative for the opposite direction. In this case, the size of the original image could be changed after rotating the image, so you have to specify `Resize proportionally` boolean parameter to indicate should the resulting image resized proportionally or not. Additionally, you could specify the background color to fill empty corners of the rotated image.
</p>

{% gist aspose-com-gists/7ee37a401e37790396ad9f4cde87d446 rotate-image-on-specific-angle.cs %}
