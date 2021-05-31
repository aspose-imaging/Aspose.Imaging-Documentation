---
title: Crop, Rotate and Resize Images
type: docs
weight: 60
url: /java/crop-rotate-and-resize-images/
---

## **Cropping Raster Images**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used for to cut out some portion of an image to increase the focus on a particular area. From Aspose.Imaging 2.4.0, the API supports two different approaches to image cropping: by [shifts](#cropping-by-shifts) and [rectangle](#cropping-by-rectangle).

### **Cropping by Shifts**
The [RasterImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage) class provides an overloaded version of the [Crop](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#crop-int-int-int-int-) method that accepts 4 integer values denoting Left, Right, Top & Bottom. Based on these four values, the [Crop](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#crop-com.aspose.imaging.Rectangle-) method moves the image boundaries toward the center of the image while discarding the outer portion. The code snippet below demonstrates how to crop an image by shifts.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Jpeg-CroppingByShifts.java" >}}


### **Cropping by Rectangle**
The [RasterImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage) class provides another overloaded version of the [Crop](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Rectangle) method that accepts an instance of the [Rectangle](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Rectangle) class. You can cut out any portion of an image by providing the desired boundaries to the [Rectangle](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Rectangle) object. The code snippet below demonstrates how to Crop any image by Rectangle.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Jpeg-CroppingByRectangle.java" >}}

## **Cropping Vector Images**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Aspose.Imaging supports cropping of vector images. Below we demonstrate cropping of svg image.

### **Crop svg Image**
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Crop-svg-image.java" >}}

## **Rotate and Flip an Image**
Aspose.Imaging for Java is an easy to use library because it provides simple methods to perform complex operations while encapsulating all ugly details. For instance, Aspose.Imaging for Java has provided [rotateFlip](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#rotateFlip-int-) method for it's base class [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) if an application requires rotating an image. Irrespective of the image format, the library can perform specific **Rotate & Flip** procedure on it.

### **Rotating an Image**
The Image.rotateFlip method can be used to rotate the image by 90/180/270-degrees and flip the image horizontally or vertically. Image.rotateFlip method accepts a parameter of [RotateFlipType](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RotateFlipType) that specifies the type of rotation and flip to apply to the image. The steps to perform **Rotate & Flip** are as simple as below,

1. Load in image using the factory method [Load](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image/methods/load/index) exposed by [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) class.
1. Call the Image.RotateFlip method while specifying the appropriate [RotateFlipType](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RotateFlipType).
1. Save the results.

The following code example demonstrates how to set the [RotateFlip](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#rotateFlip-int-) property of an [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) and the [RotateFlipType](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RotateFlipType) enumeration.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingAnImage-RotatingAnImage.java" >}}

**RotateFlipType Enumeration**

Members of RotateFlipType class and their details are outlined as follow.
More information see [here](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RotateFlipType).

|**Member**|**Description**|
| :- | :- |
|**Rotate180FlipNone**|Specifies a 180-degree clockwise rotation without flipping.|
|**Rotate180FlipX**|Specifies a 180-degree clockwise rotation followed by a horizontal flip.|
|**Rotate180FlipXY**|Specifies a 180-degree clockwise rotation followed by a horizontal and vertical flip.|
|**Rotate180FlipY**|Specifies a 180-degree clockwise rotation followed by a vertical flip.|
|**Rotate270FlipNone**|Specifies a 270-degree clockwise rotation without flipping.|
|**Rotate270FlipX**|Specifies a 270-degree clockwise rotation followed by a horizontal flip.|
|**Rotate270FlipXY**|Specifies a 270-degree clockwise rotation followed by a horizontal and vertical flip.|
|**Rotate270FlipY**|Specifies a 270-degree clockwise rotation followed by a vertical flip.|
|**Rotate90FlipNone**|Specifies a 90-degree clockwise rotation without flipping.|
|**Rotate90FlipX**|Specifies a 90-degree clockwise rotation followed by a horizontal flip.|
|**Rotate90FlipXY**|Specifies a 90-degree clockwise rotation followed by a horizontal and vertical flip.|
|**Rotate90FlipY**|Specifies a 90-degree clockwise rotation followed by a vertical flip.|
|**RotateNoneFlipNone**|Specifies no rotation and no flipping.|
|**RotateNoneFlipX**|Specifies no rotation followed by a horizontal flip.|
|**RotateNoneFlipXY**|Specifies no rotation followed by a horizontal and vertical flip.|
|**RotateNoneFlipY**|Specifies no rotation followed by a vertical flip.|


## **Rotating an Image on a Specific Angle**
From version 2.5.0, the Aspose.Imaging for Java API has exposed the RasterImage.Rotate method to facilitate its users who wish to rotate an image on a specific angle. Unlike the [RasterImage.rotateFlip](http://www.aspose.com/api/java/imaging/aspose.imaging/image/methods/rotateflip) method, the RasterImage.rotate method accepts three parameters:

1. Rotation angle: A float type parameter that specifies the rotation angle to which the image has to be rotated. A positive value rotates the image clockwise; a negative value performs an anticlockwise rotation.
1. Resize proportionally: A Boolean type parameter specifies if the image size has to changed according to the rotated rectangle (corner points) projections. If set to false, the image dimensions would be untouched and only internal image contents are rotated.
1. Background color: A Color type parameter specifies the color to be filled in the background of the rotated image.

The code snippet below demonstrates the usage of RasterImage.Rotate method.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-RotatingImageOnSpecificAngle-RotatingImageOnSpecificAngle.java" >}}

From version 2.5.0, the Aspose.Imaging for Java API has exposed the RasterImage.Rotate method to facilitate its users who wish to rotate an image on a specific angle.


## **Resizing raster Images**
This article demonstrates the usage of Aspose.Imaging for Java to perform **Resize** operation on raster image. Aspose.Imaging APIs have exposed efficient & easy to use methods to achieve this goal. Aspose.Imaging for Java has exposed the Resize method for the [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) class that can be used to re-size existing images on the fly. There are two overloads of the Resize method to suit the application needs.
### **Resizing Images : Simple Resizing**
The steps to perform **Resize** are as simple as below,

1. Load in image using the factory method [load](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#load-java.lang.String-) exposed by [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image)  class.
1. Call the Image.resize method while specifying new Height & Width.
1. Save the results.

The following code example demonstrates how to Resize an image.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-SimpleResizing-SimpleResizing.java" >}}


### **Resizing Images : Resizing with ResizeType Enumeration**
Aspose.Imaging API has exposed [ResizeType enumeration](https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType) that can be used with Image.resize to achieve desired results. Below provided code snippet demonstrates the usage of [ResizeType enumeration](https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType), whereas the details of [ResizeType enumeration](https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType) members can be found at the bottom of this page.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ResizeImageWidthwithResizeTypeEnumeration-ResizeImageWidthwithResizeTypeEnumeration.java" >}}

If you intend to get quality result after applying the re-size then it is suggested that you should always use ResizeType.LanczosResample because it will output highly qualitative results but may work slower than ResizeType.NearestNeighbourResample. On the other hand, ResizeType.NearestNeighbourResample algorithm is specifically used for fast re-sizing while compromising on the image quality. This method may be useful for thumbnail generation in real time or similar processes where performance is required.

### **Resizing Images : ResizeType Enumeration**
ResizeType determines the type of re-sizing to be performed on the image based on the selected filter.

Members of ResizeType Enumeration

|**Member Name**|**Value**|**Description**|
| :- | :- | :- |
|LeftTopToLeftTop|0|Left top point of the new image will coincide with the left top point of the original image. Crop will occur if required.|
|RightTopToRightTop|1|Right top point of the new image will coincide with the right top point of the original image. Crop will occur if required.|
|RightBottomToRightBottom|2|Right bottom point of the new image will coincide with the right bottom point of the original image. Crop will occur if required.|
|LeftBottomToLeftBottom|3|Left bottom point of the new image will coincide with the left bottom point of the original image. Crop will occur if required.|
|CenterToCenter|4|Center of the new image will coincide with the center of the original image. Crop will occur if required.|
|LancrosResample|5|Resample using lancros algorithm using 7x7 mask.|
|NearestNeighbourResample|6|Resample using nearest neighbour algorithm.|

### **Resize webp image**
Using Aspose.Imaging you can easizy resize webp image. Below we provide example of such convertion.
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Resize-webp-image.java" >}}
  
## **Resizing vector Images**
This article demonstrates the usage of Aspose.Imaging for Java to perform **Resize** operation on vector image. As example **svg image resize** provided.

### **Resizing Svg Image**
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-SvgNativeResize.java" >}}

### **Resize Image Proportionally**
Aspose.Imaging for Java has exposed the [resizeWidthProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeWidthProportionally-int-) and [resizeHeightProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeHeightProportionally-int-) methods for the [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) class that can be used to re-size existing images on the fly while keeping the aspect ratio.

### **Simple Resizing**
The following code example demonstrates the use of [resizeWidthProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeWidthProportionally-int-) and [resizeHeightProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeHeightProportionally-int-) methods.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-SimpleResizeImageProportionally-SimpleResizeImageProportionally.java" >}}


### **Resizing with ResizeType Enumeration**
Aspose.Imaging for Java API has also exposed overload versions of the [resizeWidthProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeWidthProportionally-int-int-) and [resizeHeightProportionally](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeHeightProportionally-int-int-) methods that can accept ResizeType as second parameter to achieve desired results. Below provided code snippet demonstrates the usage of [ResizeType enumeration](https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType), whereas the details of [ResizeType enumeration](https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType) members can be found at the bottom of this page.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ResizeImageWidthwithResizeTypeEnumeration-ResizeImageWidthwithResizeTypeEnumeration.java" >}}

### **ResizeType Enumeration**
ResizeType determines the type of re-sizing to be performed on the image based on the selected filter.

### **Members of ResizeType Enumeration**
ResizeType determines the type of re-sizing to be performed on the image based on the selected filter.

**Members of ResizeType Enumeration**

|**Member Name**|**Value**|**Description**|
| :- | :- | :- |
|LeftTopToLeftTop|0|Left top point of the new image will coincide with the left top point of the original image. Crop will occur if required.|
|RightTopToRightTop|1|Right top point of the new image will coincide with the right top point of the original image. Crop will occur if required.|
|RightBottomToRightBottom|2|Right bottom point of the new image will coincide with the right bottom point of the original image. Crop will occur if required.|
|LeftBottomToLeftBottom|3|Left bottom point of the new image will coincide with the left bottom point of the original image. Crop will occur if required.|
|CenterToCenter|4|Center of the new image will coincide with the center of the original image. Crop will occur if required.|
|LancrosResample|5|Resample using lancros algorithm using 7x7 mask.|
|NearestNeighbourResample|6|Resample using nearest neighbour algorithm.|
If you intend to get quality result after applying the re-size then it is suggested that you should always use ResizeType.LanczosResample because it will output highly qualitative results but may work slower than ResizeType.NearestNeighbourResample. On the other hand, ResizeType.NearestNeighbourResample algorithm is specifically used for fast re-sizing while compromising on the image quality. This method may be useful for thumbnail generation in real time or similar processes where performance is required.
