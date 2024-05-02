---
title: Crop, Rotate and Resize Images
type: docs
weight: 50
url: /ru/python-net/crop-rotate-and-resize-images/
---

## **Cropping Raster Images**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used for to cut out some portion of an image to increase the focus on a particular area. From Aspose.Imaging 2.3.0, the API supports two different approaches to image cropping: by shifts and rectangle.

### **Cropping by Shifts**
The [RasterImage](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage) class provides an overloaded version of the [crop](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/) method that accepts 4 integer values denoting Left, Right, Top & Bottom. Based on these four values, the [crop](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/) method moves the image boundaries toward the center of the image while discarding the outer portion. The code snippet below demonstrates how to crop an image by shifts.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "cropping-by-shifts.py" >}}

### **Cropping by Rectangle**
The [RasterImage](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage) class provides another overloaded version of the [crop](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/) method that accepts an instance of the [Rectangle](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rectangle) class. You can cut out any portion of an image by providing the desired boundaries to the Rectangle object. The code snippet below demonstrates how to Crop any image by Rectangle.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "cropping-by-rectangle.py" >}}

## **Cropping Vector Images**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Aspose.Imaging supports cropping of vector images. Below we demonstrate cropping of svg image.

### **Crop svg Image**
{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "crop-svg-image.py" >}}

## **Rotate and Flip an Image**
Aspose.Imaging for Python via .NET is an easy to use library because it provides simple methods to perform complex operations while encapsulating all ugly details. For instance, Aspose.Imaging for Python via .NET has provided [RotateFlip](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) method for it's base class [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) if an application requires rotating an image. Irrespective of the image format, the library can perform specific **Rotate & Flip** procedure on it.

### **Rotating an Image**
The Image.RotateFlip method can be used to rotate the image by 90/180/270-degrees and flip the image horizontally or vertically. Image.RotateFlip method accepts a parameter of [RotateFlipType](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype) that specifies the type of rotation and flip to apply to the image. The steps to perform **Rotate & Flip** are as simple as below,

1. Load in image using the factory method [load](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/methods) exposed by [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class.
1. Call the Image.RotateFlip method while specifying the appropriate [RotateFlipType](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype).
1. Save the results.

The following code example demonstrates how to set the [RotateFlip](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/methods/rotateflip) property of an [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) and the [RotateFlipType](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype) enumeration.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "rotate-image.py" >}}

**RotateFlipType Enumeration**

Members of [RotateFlipType](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype) enumeration and their details are [available here](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rotatefliptype).
## **Rotating an Image on a Specific Angle**
From version 2.5.0, the Aspose.Imaging API has exposed the RasterImage.rotate method to facilitate its users who wish to rotate an image on a specific angle. Unlike the [RasterImage.RotateFlip](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/methods/rotateflip) method, the RasterImage.rotate method accepts three parameters:

1. Rotation angle: A float type parameter that specifies the rotation angle to which the image has to be rotated. A positive value rotates the image clockwise; a negative value performs an anticlockwise rotation.
1. Resize proportionally: A Boolean type parameter specifies if the image size has to changed according to the rotated rectangle (corner points) projections. If set to false, the image dimensions would be untouched and only internal image contents are rotated.
1. Background color: A Color type parameter specifies the color to be filled in the background of the rotated image.

The code snippet below demonstrates the usage of RasterImage.Rotate method.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "rotate-image-on-specific-angle.py" >}}

From version 2.5.0, the Aspose.Imaging API has exposed the RasterImage.rotate method to facilitate its users who wish to rotate an image on a specific angle.

## **Resizing raster Images**
This article demonstrates the usage of Aspose.Imaging for Python via .NET to perform **Resize** operation on raster image. Aspose.Imaging APIs have exposed efficient & easy to use methods to achieve this goal. Aspose.Imaging for Python via .NET has exposed the Resize method for the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class that can be used to re-size existing images on the fly. There are two overloads of the resize method to suit the application needs.

### **Resizing Images : Simple Resizing**
The steps to perform **Resize** are as simple as below,

1. Load in image using the factory method [load](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) exposed by [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class.
1. Call the Image.Resize method while specifying new Height & Width.
1. Save the results.

The following code example demonstrates how to Resize an image.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "simple-resizing-image.py" >}}

### **Resizing Images : Resizing with ResizeType Enumeration**
Aspose.Imaging API has exposed [ResizeType enumeration](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype) that can be used with Image.resize to achieve desired results. Below provided code snippet demonstrates the usage of [ResizeType enumeration](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype), whereas the details of [ResizeType enumeration](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype) members can be found at the bottom of this page.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-with-resize-type.py" >}}

If you intend to get quality result after applying the re-size then it is suggested that you should always use ResizeType.LANCZOS_RESAMPLE because it will output highly qualitative results but may work slower than ResizeType.NEAREST_NEIGHBOUR_RESAMPLE. On the other hand, ResizeType.NEAREST_NEIGHBOUR_RESAMPLE algorithm is specifically used for fast re-sizing while compromising on the image quality. This method may be useful for thumbnail generation in real time or similar processes where performance is required.

### **Resizing Images : ResizeType Enumeration**
ResizeType determines the type of re-sizing to be performed on the image based on the selected filter.

Members of ResizeType Enumeration

|**Member Name**|**Value**|**Description**|
| :- | :- | :- |
|LEFT_TOP_TO_LEFT_TOP|0|Left top point of the new image will coincide with the left top point of the original image. Crop will occur if required.|
|RIGHT_TOP_TO_RIGHT_TOP|1|Right top point of the new image will coincide with the right top point of the original image. Crop will occur if required.|
|RIGHT_BOTTOM_TO_RIGHT_BOTTOM|2|Right bottom point of the new image will coincide with the right bottom point of the original image. Crop will occur if required.|
|LEFT_BOTTOM_TO_LEFT_BOTTOM|3|Left bottom point of the new image will coincide with the left bottom point of the original image. Crop will occur if required.|
|CENTER_TO_CENTER|4|Center of the new image will coincide with the center of the original image. Crop will occur if required.|
|LANCZOS_RESAMPLE|5|Resample using lancros algorithm using 7x7 mask.|
|NEAREST_NEIGHBOUR_RESAMPLE|6|Resample using nearest neighbour algorithm.|

### **Resize webp image**
Using Aspose.Imaging you can easizy resize webp image. Below we provide example of such convertion.
{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-webp-image.py" >}}

## **Resizing vector Images**
This article demonstrates the usage of Aspose.Imaging for Python via .NET to perform **Resize** operation on vector image. As example **svg image resize** provided.

### **Resize svg Image**
{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "svg-native-resize.py" >}}

## **Resize Image Proportionally**
You can [resize images]() by passing new height & width values as parameters to the Image.Resize method but in that case you have to calculate the aspect ratio yourself. This is because when the width or height of an image is altered, the image is either scaled or shrinked to fill the new size . If the changes to the width and height of an image are not in proportion this can lead to stretched and distorted result. This article demonstrates the use of Aspose.Imaging for Python via .NET API to resize images by passing either new height or width while allowing the API to automatically calculate the other proportional value.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-image-proportionally.py" >}}

### **Resize Image Proportionally**
Aspose.Imaging for Python via .NET has exposed the [resize_width_proportionally]() and [resize_height_proportionally]() methods for the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class that can be used to re-size existing images on the fly while keeping the aspect ratio.

### **Simple Resizing**
The following code example demonstrates the use of [resize_width_proportionally](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) and [resize_height_proportionally](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) methods.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-image-proportionally.py" >}}

### **Resizing with ResizeType Enumeration**
Aspose.Imaging for Python via .NET API has also exposed overload versions of the [resize_width_proportionally](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) and [resize_height_proportionally](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) methods that can accept ResizeType as second parameter to achieve desired results. Below provided code snippet demonstrates the usage of [ResizeType enumeration](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype), whereas the details of [ResizeType enumeration](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype) members can be found at the bottom of this page.

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-image-with-resize-type-enumeration.py" >}}

### **ResizeType Enumeration**
ResizeType determines the type of re-sizing to be performed on the image based on the selected filter.

### **Members of ResizeType Enumeration**

|**Member Name**|**Value**|**Description**|
| :- | :- | :- |
|LEFT_TOP_TO_LEFT_TOP|0|Left top point of the new image will coincide with the left top point of the original image. Crop will occur if required.|
|RIGHT_TOP_TO_RIGHT_TOP|1|Right top point of the new image will coincide with the right top point of the original image. Crop will occur if required.|
|RIGHT_BOTTOM_TO_RIGHT_BOTTOM|2|Right bottom point of the new image will coincide with the right bottom point of the original image. Crop will occur if required.|
|LEFT_BOTTOM_TO_LEFT_BOTTOM|3|Left bottom point of the new image will coincide with the left bottom point of the original image. Crop will occur if required.|
|CENTER_TO_CENTER|4|Center of the new image will coincide with the center of the original image. Crop will occur if required.|
|LANCZOS_RESAMPLE|5|Resample using lancros algorithm using 7x7 mask.|
|NEAREST_NEIGHBOUR_RESAMPLE|6|Resample using nearest neighbor algorithm.|
If you intend to get quality result after applying the re-size then it is suggested that you should always use ResizeType.LanczosResample because it will output highly qualitative results but may work slower than ResizeType.NEAREST_NEIGHBOUR_RESAMPLE. On the other hand, ResizeType.NEAREST_NEIGHBOUR_RESAMPLE algorithm is specifically used for fast re-sizing while compromising on the image quality. This method may be useful for thumbnail generation in real time or similar processes where performance is required.
