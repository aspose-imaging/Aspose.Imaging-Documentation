---
title: Manipulating DICOM Formats
type: docs
weight: 30
url: /ru/python-net/manipulating-dicom-formats/
---

## **Adjusting Brightness, Contrast and Gamma**
Color adjustments in digital images is one of the core features that most of the imaging libraries provide. Color adjustments can be categorized in the following.

1. **Brightness** refers to the lightness or darkness of color. Increasing the brightness of an image lights out all colors whereas decreasing the brightness darkens all colors.
1. **Contrast** refers to making the objects or details within an image more obvious. Increasing the contrast of an image increases the difference between light and dark areas so that the light areas becomes lighter and dark areas becomes darker. Decreasing the contrast will make lighter and darker areas stay approximately the same but the overall image becomes more homogeneous.
1. **Gamma** optimizes the contrast and brightness of the indirect lighting that is illuminating an object in the image.

### **Adjusting Brightness**
Aspose.Imaging for Python via .NET API provide adjust_brightness method for the DicomImage class that can be used to adjust the **Brightness** by passing an integer value as parameter.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "adjust-brightness-dicom.py" >}}

### **Adjusting Contrast**
The adjust_contrast method exposed by the DicomImage class can be used to adjust the **Contrast** of an image by passing a float value as parameter.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "adjust-contrast-dicom.py" >}}

### **Adjusting Gamma**
The adjust_gamma method exposed by the DicomImage class can be used to adjust the **Gamma** of an image by passing a float value as parameter.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "adjust-gamma-dicom.py" >}}

## **Applying Filters**
This article demonstrates the usage of Aspose.Imaging for Python via .NET to apply filter on a DICOM image. Aspose.Imaging APIs have exposed efficient & easy to use methods to achieve this goal. The following code example demonstrates how to apply filter on DICOM image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "apply-filter-dicom.py" >}}

## **Applying Binarization**
In order to understand the concept of Binarization, it is important to define a Binary Image; that is a digital image that can have only two possible values for each pixel. Normally, the two colors used for a binary image are black and white though any two colors can be used. Binarization is the process of converting an image to bi-level meaning that each pixel is stored as a single bit (0 or 1) where 0 denotes the absence of color and 1 means presence of color. Aspose.Imaging for Python via .NET API supports three different methods of binarization for DICOM images.

### **Using Fixed Threshold**
Following code snippet demonstrates how Fixed Threshold Binarization can be applied to a DICOM image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "binarize-with-fixed-threshold-dicom.py" >}}

### **Using Otsu Threshold**
Following code snippet demonstrates how Otsu Threshold Binarization can be applied to a DICOM image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "binarize-with-otsu-threshold-dicom.py" >}}


### **Using Bradley's Adaptive Threshold**
Following code snippet demonstrates how Bradley's Adaptive Threshold Binarization can be applied to a DICOM image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "binarize-with-otsu-threshold-dicom.py" >}}


### **Using Grayscaling**
Gray-scaling is the process of converting a continuous-tone image to an image with discontinues gray shades.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "grayscale-dicom.py" >}}


## **Cropping Image**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used to take out some portion of an image to increase the focus on a particular area. Aspose.Imaging for Python via .NET API now supports DICOM image cropping.

## **Cropping by Shifts**
The DicomImage class provides the **crop** method that accepts 4 integer values. Based on these four values, the Crop method take out that part of the image while discarding the rest of the image. The code snippet below demonstrates how to crop a DICOM image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "crop-by-shifts-dicom.py" >}}

## **Dithering For DICOM Image**
Dithering is a technique of creating the illusion of new colors and shades by varying the pattern of dots that actually create an image. It is the most common means of reducing the color range of images down to the 256 (or fewer) colors. Aspose.Imaging provides the dithering support for DicomImage class by introducing Dither method that accepts two parameters. First is of type DitheringMethod to be applied with two possible options FLOYD_STEINBERG_DITHERING and THRESHOLD_DITHERING. The second parameter to dither method is the BitCount in integer. BitCount defines the sampling size for the dithering result. Default value is 1 that represents black and white, whereas allowed values are 1, 4, 8 generating palettes with 2, 4 and 256 colors respectively.

## **Resizing DICOM Image**
This article demonstrates the usage of Aspose.Imaging for Python via .NET to perform Resize operation on a DICOM image. Aspose.Imaging APIs have exposed efficient & easy to use methods to achieve this goal. Aspose.Imaging for Python via .NET has exposed the **resize** method of the **DicomImage** class that can be used to re-size existing images on the fly. The steps to perform Resize are as simple as below:

1. Load in image using the constructor of the **DicomImage** class.
1. Call the DicomImage.resize method while specifying new Height & Width.
1. Save the results.

### **Simple Resizing**
The following code example demonstrates how to resize an image.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "simple-resize-dicom.py" >}}

### **Other Resizing Options**
Aspose.Imaging API has exposed **resize_height_proportionally** and **resize_width_proportionally** methods of the **DicomImage** class that can be used to re-size the DICOM images. These methods take in an integer as first argument and **ResizeType** enumeration to achieve desired results. Below provided code snippet demonstrates the usage of these methods.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "other-resize-options-dicom.py" >}}

## **Rotate and Flip DICOM Image**
Aspose.Imaging for .NET has provided **rotate** and **rotate_flip** methods of **DicomImage** class to rotate/flip a DICOM image. The **DicomImage.rotate** method can be used to rotate the image. The **rotate** method take an integer parameter as degrees to rotate. **DicomImage.rotate_flip** method accepts a parameter of RotateFlipType that specifies the type of rotation and flip to apply to the image. The steps to perform Rotate & Flip are as simple as below:

1. Load in image using the **DicomImage** class constructor.
1. Call the **DicomImage.rotate_flip** or **DicomImage.rotate** method while specifying the appropriate parameter.
1. Save the results.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "rotate-dicom.py" >}}

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "flip-dicom.py" >}}

## **Export to DICOM**
Aspose.Imaging supports export from various raster file formats including multi-paged to DICOM. Below there are some examples related to this.

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "export-to-dicom.py" >}}

## **Support of Jpeg, Jpeg2000 and RLE compression methods in Dicom**
Dicom format can be compressed using Jpeg, Jpeg2000 and RLE compressions.
{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "jpeg-jpeg2000-rle-compressions-dicom.py" >}}

## **Memory strategy optimization**
The memory optimization strategy is now supported for Dicom images.

Here are some examples of its use:

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "memory-strategy-optimization-dicom.py" >}}

## **Add xmp tags to dicom image**
Using Aspose.Imaging you can easily add xmp tags to dicom image.

Here is example of usage:

{{< gist "aspose-com-gists" "e4d41a92dd100ad966dc888bc9528155" "add-xmp-tags-to-dicom-image.py" >}}
