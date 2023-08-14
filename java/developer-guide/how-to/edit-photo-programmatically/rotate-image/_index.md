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
Rotating an image with a fixed angle of 90/180/270-degree with or without a flip can be done with <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/#rotateFlip-int-">RotateFlip method</a>. You need to pass a rotate type parameter to the method. In the Java code example below we use the type `Rotate270FlipNone`:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingAnImage-RotatingAnImage.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Please refer to the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rotatefliptype/">Rotate and flip types parameters</a> list for available rotating types.
</p>

### Rotate an image to the specific angle

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Additionally, you can rotate an image to a specific angle with <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#rotate-float-">Rotate method</a>. For clockwise rotation, the rotation angle value should be positive and for the opposite direction - negative. Also, you can use <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#rotate-float-boolean-com.aspose.imaging.Color-">Rotate method with additional parameters</a>. `Resize proportionally` boolean parameter indicates whether the resulting image resizes proportionally or not. Otherwise, empty corners will appear after the image was rotated and you need to indicate the background color to fill the corners.
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingImageOnSpecificAngle-RotatingImageOnSpecificAngle.java" >}}
