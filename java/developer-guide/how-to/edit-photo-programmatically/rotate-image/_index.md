---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/rotate-image
linktitle: How to rotate an image
title: How to rotate an image
description: Rotate an image to a fixed angle. Flip images vertically or horizontally. Rotate photos to a selected angle.
keywords: [rotate an image, rotating image, flip an image]
---

## How to rotate an image

### Rotate and flip an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The first type of rotating image is a rotation to a fixed angle of 90/180/270-degree with or without a flip. You just need to load your image and apply the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/#rotateFlip-int-">RotateFlip method</a> with a rotate type parameter. We use the type `Rotate270FlipNone` in this example:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingAnImage-RotatingAnImage.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a full list of available types please see the link to the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rotatefliptype/">rotate and flip types parameters</a> descriptions.
</p>

### Rotate an image to the arbitrary angle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The second type is rotating for an arbitrary choice angle with <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#rotate-float-">Rotate method</a>. The rotation angle value could be positive if a rotation is clockwise or negative for the opposite direction. Also, you can use <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#rotate-float-boolean-com.aspose.imaging.Color-">Rotate method with additional parameters</a>. In this case, the size of the original image could be changed after rotating the image, so you have to specify `Resize proportionally` boolean parameter to indicate should the resulting image resized proportionally or not. Additionally, you could specify the background color to fill empty corners of the rotated image.
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingImageOnSpecificAngle-RotatingImageOnSpecificAngle.java" >}}
