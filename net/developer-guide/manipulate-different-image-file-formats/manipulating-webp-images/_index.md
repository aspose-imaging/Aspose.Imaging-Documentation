---
title: Manipulating WebP Images
type: docs
weight: 170
url: /net/manipulating-webp-images/
---

## **Convert GIFF Image Frame to WebP Image**
Aspose.Imaging enables you to extract a frame or frames from any existing **GIFF** image and convert it to **WebP** format. This article shows how you can extract a particular frame from a **GIFF** image and convert it to a **WebP** image. Following are the steps to convert a **GIFF** frame to a **WebP** image.

1. Load an existing **GIFF** image into an instance of **Image** using the factory method Load.
1. Create and initialize an instance of **GifImage** class.
1. Create and initialize an instance of [WebPImage](https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.webp/webpimage) class.
1. Access the **GIFF** image Frame with [GifImage](https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.gif/gifimage) property.
1. Create and initialize an instance of [WebPFrameBlock](https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.webp/webpframeblock) class.
1. Add WebP frame to WebP image block list.
1. Set **WebP** image options.
1. Save **WebP** image.

Following is the code demonstration.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-ConvertGIFFImageFrame-ConvertGIFFImageFrame.cs" >}}


## **Create WebP Image**
WebP is a new image format that provides lossless and lossy compression for images on the web. Developers can use the WebP image format to create smaller and richer images that can help make the web faster. Using Aspose.Imaging for .NET API developers can create WebP image. This article demonstrates the use of [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) and **Image** classes to create a WebP image. The release of Aspose.Imaging for .NET 3.3.0 contains the [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) class. With the help of [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) class developer can create **WebP** image. The code snippet provided below demonstrates how to use it.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-CreatingWebPImage-CreatingWebPImage.cs" >}}


## **Exporting Image to WebP**
Aspose.Imaging lets you save files in Webp format. This article shows how to save a file in Webp format with Aspose.Imaging, and it also discusses some of the settings that can be used when saving to this format. [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) is a specialized class in the [ImageOptions](https://apireference.aspose.com/imaging/net/aspose.imaging/imageoptionsbase) namespace used to manipulate **WebP** images. To export to Webp, create an instance of the [Image](http://www.aspose.com/api/net/imaging/aspose.imaging/image) class, either loaded from an existing image file or created from scratch. This article explains how. In the example below, an existing image is loaded by passing the file path to the [Image](http://www.aspose.com/api/net/imaging/aspose.imaging/image) class static Load method. Once it is loaded, save the image using the [Image](http://www.aspose.com/api/net/imaging/aspose.imaging/image) class [Save](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/save/index) method, and supply a [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) object as the second argument [WebPOptions](https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/webpoptions) class properties can be set while conversion. Some of the properties are Quality and Lossless. Following is the code demonstration.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-ExportToWebP-ExportToWebP.cs" >}}


## **Exporting WebP to Other Image Formats**
Using Aspose.Imaging you can convert **WebP** image to other image formats. This article shows how you can convert a **WebP** image to other image format. In the example below, an existing **WebP** image is loaded by passing the file path to the [Image](http://www.aspose.com/api/net/imaging/aspose.imaging/image) class static Load method. Once it is loaded, save the image using the [Image](http://www.aspose.com/api/net/imaging/aspose.imaging/image) class [Save](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/save/index) method, and supply a instance of [BmpOptions]() as the second argument. In this way a **WebP** image will be converted to a **BMP** image.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-ExportWebPToOtherImageFormats-ExportWebPToOtherImageFormats.cs" >}}


## **Extract Frames From WebP Image**
Aspose.Imaging enables you to extract a frame or frames from any existing **WebP** image and convert it to other image formats. This article shows how you can extract a particular frame from a **WebP** image and convert it to a Raster image. **Aspose.Imaging.FileFormats.Webp.WebPImage** has a property called **Blocks**. Once an existing **WebP** image is loaded, **Blocks** property will contain the array of frames inside the **WebP** image. Using **Blocks** property you can access an individual frame image. In the example below, an existing **WebP** image is loaded by passing the file path to the **Aspose.Imaging.FileFormats.Webp.WebPImage** class. Once it is loaded, check the **Blocks** property. If it is greater then zero then it means frames inside the **WebP** image have been loaded. Now access a particular frame and convert it into any Raster Image.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-ExtractFrameFromWebPImage-ExtractFrameFromWebPImage.cs" >}}
## **Update WebP Image**
There was an **OutOfMemoryException** when saving WebP file after resize, crop and rotate&flip actions. Aspose.Imaging for .NET provides a simple solution to self-update WebP image. The following code snippet shows how to update the WebP file.

{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "Examples-CSharp-ModifyingAndConvertingImages-WebPImages-OpenWebPFile-OpenWebPFile.cs" >}}
## **Memory Strategy Optimization**
Load and create of WebP images can be proceeded using memory strategy optimization - ie limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "MemoryStrategyOptimizationWebP.cs" >}}
## **Batch export to WebP**
**Batch (sequential) export mode at all**

Batch (or sequential) export mode eliminates the need to store the data of all pages of a multi-page image in memory.

This approach implements the idea of "Loading a page into memory from an input stream --> processing a page (for example, a rotation operation) --> exporting a page to an output stream --> freeing memory --> loading the next page, and so on".

The Aspose.Imaging currently supports batch export in the following formats:

- For source images: Tiff, Djvu (i.e. only TiffImage and DjvuImage can be processed in batch export mode);
- In image exporters: Tiff, Gif, Apng, Dicom, WebP.

In this way batch exports are currently supported in the following combinations:

- from Tiff to Tiff;
- from Tiff to Gif;
- from Tiff to Apng;
- from Tiff to Dicom;
- from Tiff to WebP;
- from Djvu to Tiff;
- from Djvu to Gif;
- from Djvu to Apng;
- from Djvu to Dicom;
- from Djvu to WebP.

`  `Load and create of WebP images can be proceeded using memory strategy optimization - ie limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "Examples-Batch-export-from-tiff-to-webp.cs" >}}
