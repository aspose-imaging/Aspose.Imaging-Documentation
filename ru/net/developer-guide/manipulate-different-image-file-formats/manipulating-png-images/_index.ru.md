---
title: Manipulating PNG Images
type: docs
weight: 140
url: /ru/net/manipulating-png-images/
---

## **Specifying Transparency for PNG Images**
One of the advantages of saving images in PNG format is that PNG can have transparent background. Aspose.Imaging for .NET provides the feature for specifying transparency for the [PngImage](https://reference.aspose.com/imaging/ru/net/aspose.imaging.fileformats.png/pngimage) & RasterImage classes as demonstrated in the below section. Aspose.Imaging for .NET API can be used to set any color as transparent while creating new PNG images or converting existing images to PNG format. For this purposes, the Aspose.Imaging for .NET API has exposed [TransparentColor](https://reference.aspose.com/imaging/ru/net/aspose.imaging.fileformats.png/pngimage/properties/transparentcolor) property and [PngColorType](https://reference.aspose.com/imaging/ru/net/aspose.imaging.fileformats.png/pngcolortype) enumeration that can be set to specify any color to be rendered as transparent in the newly created PNG image. The below provided code snippet demonstrates how to convert an existing BMP image to PNG format by creating a PNG image from scratch while specifying the desired color as transparent.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "specify-transparency-png.cs" >}}


## **Setting Resolution for PNG Images**
With Aspose.Imaging for .NET 2.5.0, the API exposes the [ResolutionSetting](https://reference.aspose.com/imaging/ru/net/aspose.imaging/resolutionsetting) class which can be used to set the resolution for all image formats including PNG. This article demonstrates the usage of the Aspose.Imaging for .NET API to set the horizontal & vertical resolution parameters for the PNG image format. The code snippet below loads an existing BMP image and converts it to PNG format also changing the resolution.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "set-resolution-in-png-images.cs" >}}


## **Compressing PNG Files**
The Portable Network Graphic (PNG) is a lossless compression format for transmitting a bitmap over networks. When you save an image as a PNG file in any program, you may be asked to choose a compression level in a range from 0 to any max level. Setting this value actually compresses the file size and does not decrease the image quality. This article describes how Aspose.Imaging APIs allows you to control the PNG file size. Aspose.Imaging APIs can be used to set the Compression Levels for the PNG file format using the [PngOptions](https://reference.aspose.com/imaging/ru/net/aspose.imaging.imageoptions/pngoptions) class that has an int type CompressionLevel property. This property accepts a value from 0 to 9 where 9 is the maximum compression. The below provided code snippet demonstrates how to set the Compression Levels using Aspose.Imaging for .NET API.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "compress-png-images.cs" >}}


## **Specifying Bit Depth for PNG Images**
Bit depth in imaging is the number of bits used to indicate the color of a single pixel in a bitmap image. Like all other bitmap formats, PNG color depth is also represented in bit such as 1-bit (2 colors), 2-bit (4 colors), 4-bit (16 colors) and 8-bit (256 colors). Aspose.Imaging for .NET API can be used to set bit depth for PNG images using BitDepth property exposed by the [PngOptions](https://reference.aspose.com/imaging/ru/net/aspose.imaging.imageoptions/pngoptions) class. At the moment, the BitDepth property can be set to 1, 2, 4 or 8 bits for grayscale and indexed color types. For all other color types only 8 bits are supported. The below provided code snippet demonstrates how to set the Bit Depth of an existing PNG.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "specify-bit-depth-in-png-image.cs" >}}


## **Applying Filter Methods on PNG Images**
Aspose.Imaging for .NET provides the functionality to apply filter methods (algorithms) before compression as demonstrated in the below section. The purpose of these filter methods is to prepare the image data for optimum compression. Aspose.Imaging for .NET API can be used to apply filter methods before compressing any PNG image. For this purposes, the Aspose.Imaging for .NET API has exposed a property named FilterType of [PngOptions](https://reference.aspose.com/imaging/ru/net/aspose.imaging.imageoptions/pngoptions) class. It accepts PngFilterType enumeration that can be used to specify the filter method (algorithm) among the five including 0 for none. The below provided code snippet demonstrates how to apply filter method on PNG image.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "apply-filter-method-in-png-image.cs" >}}

## **Keep transparency, when indexing Png images**
Aspose.Imaging for .NET supports keeping transparency for indexed png images on save. The following example shows how to save indexed png image and keep transparency.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "keep-transparency-when-indexing-png-image.cs" >}}

## **Changing Background Color of a Transparent PNG Image**
PNG format images can have transparent background. Aspose.Imaging for .NET provides the feature to change the background color of a PNG image that has transparent background. Aspose.Imaging for .NET API can be used to set/change color of a transparent PNG image. The below provided code snippet demonstrates how to set/change the background color of a transparent PNG image.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "change-background-color-of-transparent-png.cs" >}}
## **Optimizing Memory Usage**
When reading a big PNG file, the total amount of RAM the process will take is always a concern. There are measures which can be adopted to cope with the challenge. Aspose.Imaging provides some relevant options and API calls to lower, reduce and optimize memory use. Also, it can help the process work more efficiently and run faster.

The following example shows how to read a large PNG file in optimized mode.

{{< gist "aspose-com-gists" "0dc6787183a1823ca0774be84c7b7aa2" "memory-strategy-optimization-png.cs" >}}




