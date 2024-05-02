---
title: Manipulating WebP Images
type: docs
weight: 170
url: /ru/python-net/manipulating-webp-images/
---

## **Convert GIFF Image Frame to WebP Image**
Aspose.Imaging enables you to extract a frame or frames from any existing **GIFF** image and convert it to **WebP** format. This article shows how you can extract a particular frame from a **GIFF** image and convert it to a **WebP** image. Following are the steps to convert a **GIFF** frame to a **WebP** image.

1. Load an existing **GIFF** image into an instance of **Image** using the factory method load.
1. Create and initialize an instance of **GifImage** class.
1. Create and initialize an instance of [WebPImage](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.fileformats.webp/webpimage) class.
1. Access the **GIFF** image Frame with [GifImage](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.fileformats.gif/gifimage) property.
1. Create and initialize an instance of [WebPFrameBlock](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.fileformats.webp/webpframeblock) class.
1. Add WebP frame to WebP image block list.
1. Set **WebP** image options.
1. Save **WebP** image.

Following is the code demonstration.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "convert-gif-image-frame-to-webp.py" >}}

## **Create WebP Image**
WebP is a new image format that provides lossless and lossy compression for images on the web. Developers can use the WebP image format to create smaller and richer images that can help make the web faster. Using Aspose.Imaging for Python via .NET API developers can create WebP image. This article demonstrates the use of [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) and **Image** classes to create a WebP image. The release of Aspose.Imaging 3.3.0 contains the [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) class. With the help of [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) class developer can create **WebP** image. The code snippet provided below demonstrates how to use it.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "create-webp-image.py" >}}

## **Exporting Image to WebP**
Aspose.Imaging lets you save files in Webp format. This article shows how to save a file in Webp format with Aspose.Imaging, and it also discusses some of the settings that can be used when saving to this format. [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) is a specialized class in the [ImageOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/imageoptionsbase) namespace used to manipulate **WebP** images. To export to Webp, create an instance of the [Image](http://www.aspose.com/api/ru/python-net/imaging/aspose.imaging/image) class, either loaded from an existing image file or created from scratch. This article explains how. In the example below, an existing image is loaded by passing the file path to the [Image](http://www.aspose.com/api/ru/python-net/imaging/aspose.imaging/image) class static Load method. Once it is loaded, save the image using the [Image](http://www.aspose.com/api/ru/python-net/imaging/aspose.imaging/image) class [Save](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/methods/save/index) method, and supply a [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) object as the second argument [WebPOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/webpoptions) class properties can be set while conversion. Some of the properties are quality and lossless. Following is the code demonstration.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "export-image-to-webp.py" >}}

## **Exporting WebP to Other Image Formats**
Using Aspose.Imaging you can convert **WebP** image to other image formats. This article shows how you can convert a **WebP** image to other image format. In the example below, an existing **WebP** image is loaded by passing the file path to the [Image](http://www.aspose.com/api/ru/python-net/imaging/aspose.imaging/image) class static Load method. Once it is loaded, save the image using the [Image](http://www.aspose.com/api/ru/python-net/imaging/aspose.imaging/image) class [Save](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) method, and supply a instance of [BmpOptions]() as the second argument. In this way a **WebP** image will be converted to a **BMP** image.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "export-webp-to-other-formats.py" >}}

## **Extract Frames From WebP Image**
Aspose.Imaging enables you to extract a frame or frames from any existing **WebP** image and convert it to other image formats. This article shows how you can extract a particular frame from a **WebP** image and convert it to a Raster image. **Aspose.Imaging.FileFormats.Webp.WebPImage** has a property called **Blocks**. Once an existing **WebP** image is loaded, **Blocks** property will contain the array of frames inside the **WebP** image. Using **Blocks** property you can access an individual frame image. In the example below, an existing **WebP** image is loaded by passing the file path to the **Aspose.Imaging.FileFormats.Webp.WebPImage** class. Once it is loaded, check the **Blocks** property. If it is greater then zero then it means frames inside the **WebP** image have been loaded. Now access a particular frame and convert it into any Raster Image.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "extract-frame-from-webp-image.py" >}}

## **Update WebP Image**
There was an **OutOfMemoryException** when saving WebP file after resize, crop and rotate&flip actions. Aspose.Imaging for Python via .NET provides a simple solution to self-update WebP image. The following code snippet shows how to update the WebP file.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "open-webp-file.py" >}}

## **Memory Strategy Optimization**
Load and create of WebP images can be proceeded using memory strategy optimization - i.e. limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "8ceff50985ea61b20e58c7e4e15775f4" "memory-strategy-optimization-webp.py" >}}
