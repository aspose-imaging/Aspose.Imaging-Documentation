---
title: Manipulating TIFF Images
type: docs
weight: 240
url: /java/manipulating-tiff-images/
---

## **Add Frames with Different Settings**
TIFF is a very flexible format and it allows different frames to be added, with different dimensions, compression and other settings. Aspose.Imaging APIs allow you to add any TIFF frame of any size which helps in creating complex documents. If there is a requirement to adjust the frames during the add process to make them all equal, perform the following steps:

1. Create a new blank frame with the desired options or copy the source frame with the output options specified using the [createFrameFrom](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffFrame#createFrameFrom-com.aspose.imaging.fileformats.tiff.TiffFrame-com.aspose.imaging.imageoptions.TiffOptions-) method.
1. Resize the source frame/image to the desired dimensions using the Resize method.
1. Add the source frame/image pixels to the new frame.
1. Add the new frame to the output TIFF image.
## **Export Multi Page frames to different Image format**
Sometimes you need to export Multi-page TIFF frames to some other image file format. This article will demonstrate how we can perform this task using Aspose.Imaging for Java API. We will use [TiffImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffImage), [TiffFrame](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffFrame), [BmpOptions](https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/BmpOptions) and [BmpImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.bmp/BmpImage) classes to export TIFF frames to BMP image format. First, we will create instance of TIFF image and load images from local disk. Now we will iterate over TIFF frames and copy pixels of active frame using [loadPixels](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#loadPixels-com.aspose.imaging.Rectangle-) method into Colors array and create an instance of BmpOptions for BMP image settings. Set the desired setting for BMP image creation. Create a new BMP image using BmpOptions object and save BMP image using frame pixels, copied in Colors array.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-ExtractTIFFFramesToBMPImageFormat.java" >}}

Please note, the above provided code snippet requires setting the valid license for Aspose.Imaging for Java API. This is because Aspose.Imaging APIs restrict the usage of core features such as [loadPixels](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#loadPixels-com.aspose.imaging.Rectangle-) & [savePixels](https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#savePixels-com.aspose.imaging.Rectangle-com.aspose.imaging.Color:A-) in evaluation mode. Please check the details for [Evaluation Version Limitations](/imaging/java/licensing/).

### **Extract TIFF Frames to Other Image Format using Core Functionality**
1. Create an instance of the TIFF image and load images from local disk.
1. Iterate over the TIFF frames and copy pixels of the active frame using loadPixels method into the Colors array.
1. Create an instance of any ImageOptionsBase for desired format and set mandatory properties. For the sake of elaboration, we will use JpegOptions.
1. Create a new JPEG image using the JpegOptions object and save JPEG image using frame pixels copied in the Colors array.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-ExtractTIFFFramestoOtherImageFormatusingCoreFunctionality.java" >}}

{{% alert color="primary" %}} 

Please note, the above provided code snippet requires setting the valid license for Aspose.Imaging for Java API. This is because Aspose.Imaging APIs restrict the usage of core features such as loadPixels & savePixels in evaluation mode. Please check the details for [Evaluation Version Limitations_Imaging](/pages/createpage.action?spaceKey=imagingjava&title=Evaluation+Version+Limitations_Imaging&linkCreation=true&fromPageId=15303064).

{{% /alert %}} 
### **Extract TIFF Frames to Other Image Format**
1. Create an instance of the TiffImage and load images from local disk or stream.
1. Retrieve the collection of frames in an array of type TiffFrame.
1. Create an instance of any ImageOptionsBase for desired format and set mandatory properties. For the sake of elaboration, we will use JpegOptions.
1. Call TiffFrame.save method with destination path and an instance of appropriate ImageOptionsBase.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingTIFFImages-ExtractTIFFFramestoOtherImageFormat-ExtractTIFFFramestoOtherImageFormat.java" >}}
## **Adding Multiple images inside Tiff Frames**
This article will demonstrate how we can we add multiple images inside single tiff using Aspose.Imaging for Java API. We will use [TiffImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffImage), [TiffFrame](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffFrame) classes to add multiple images inside tiff frames. Below provided code snippet demonstrates this concept.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingTIFFImages-MultipleImageToTiff-MultipleImageToTiff.java" >}}

## **Concatenate Multiple TIFF Images**
This article exhibits the usage of Aspose.Imaging for Java API to concatenate Tiff frames to a single Tiff image. We will use TiffImage and TiffFrame classes to concatenate multiple TIFF frames. We can use both standard methods, from file and from stream, to concatenate TIFF images.
### **Images Having Single Frame**

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-images-ConcatTIFFImages-ConcatTIFFImages.java" >}}

#### **Concatenating Images from Disk**
Firstly, we will create instances of images and load images from the local disk, then we will copy the active frame of source image using [Copyframe](http://www.aspose.com/api/java/imaging/aspose.imaging.fileformats.tiff/tiffframe/methods/copyframe) method of [TiffFrame](http://www.aspose.com/api/java/imaging/aspose.imaging.fileformats.tiff/tiffframe) class and add that copied frame to destination image with the help of [Addframe](http://www.aspose.com/api/java/imaging/aspose.imaging.fileformats.tiff/tiffimage/methods/addframe) method of [TiffImage](http://www.aspose.com/api/java/imaging/aspose.imaging.fileformats.tiff/tiffimage) class. Finally we will save image back to local disk.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-images-ConcatTIFFImages-ConcatTIFFImages.java" >}}
### **Images Having Several Frames**
Below provided sample demonstrates the usage of Aspose.Imaging for Java API to concatenate Tiff images that could have several frames. For demonstration purposes, we will read a list of Tiff images, and create a new Tiff image that will hold the frames from all read Tiff images.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-ConcatenateTiffImagesHavingSeveralFrames.java" >}}

### **Add Different Images as Separate Frames in a Multi-Page TIFF**
TIFF is a flexible format allowing different frames to be added, with different dimensions, compression and other settings. This example demonstrates the usage of Aspose.Imaging for Java API to accomplish this task with core functionality.

In order to demonstrate the usage of Aspose.Imaging for Java API to add different images as frames to the resultant TIFF image, we will iterate over a list of files (.jpg) and convert them to TiffFrame before adding to the resultant TiffImage.

The following code snippet re-size all loaded images before adding them to the TiffImage

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingTIFFImages-AddDifferentImagesasSeparateFramesinaMultiPageTIFF-AddDifferentImagesasSeparateFramesinaMultiPageTIFF.java" >}}

Please note, the above provided code snippet requires setting the valid license for Aspose.Imaging for Java API. This is because Aspose.Imaging APIs restrict the usage of core features such as loadPixels & savePixels in evaluation mode. Please check the details for [Evaluation Version Limitations_Imaging](/pages/createpage.action?spaceKey=imagingjava&title=Evaluation+Version+Limitations_Imaging&linkCreation=true&fromPageId=15303064).

## **Data Recovery Options**
Sometimes you may encounter a TIFF image that cannot be rendered properly while using traditional image viewers such as Windows Photo Viewer because the image is damaged or corrupted. When loaded with Aspose.Imaging, such images may throw exceptions and you may not be able to process them further.

Aspose.Imaging for Java 2.4.0 and later supports data recovery modes for TIFF images. The data recovery allows you to load a TIFF file that has improper data layout or corrupted data strips. Data recovery replaces the corrupted data with any color specified, and you can retrieve the rest of the data for further processing without experiencing any exception.

{{% alert color="primary" %}} 

This mechanism is especially useful for TIFF file format since it stores the data in strips. When a strip is damaged the other strips may still retain the correct information.

{{% /alert %}} 

Aspose.Imaging provides two recovery modes which provide different results.

1. ConsistentRecover: The consistent recovery mode tries to recover all data as long as corruption does not break the file format and allows further processing.
1. MaximalRecover: The maximal recovery mode recovers all data even if the file format has a corrupted structure and further processing may yield unexpected effects.

Below is sample code that shows how to use the data recovery mode.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingTIFFImages-DataRecovery-DataRecovery.java" >}}

When a damaged or corrupted TIFF file is loaded or saved without using data recovery you may get an error of type com.aspose.imaging.exceptions.CompressorException.


## **TiffOptions Configuration**
Developers can adjust different properties of TiffOptions class to get desired results. In this document, we will focus on 4 main properties that controls the resultant image attributes.

These properties are listed below.

1. TiffOptions.Photometric
1. TiffOptions.Compression
1. TiffOptions.BitsPerSample
1. TiffOptions.Predictor

{{% alert color="primary" %}} 

Whenever we initialize an empty TiffOptions structure, each option is set to its default value. For instance compression is set to None, BitsPerSample is set as 1 and Photometric as MinIsWhite. Saving into this format will make the final image black n white and this is expected behavior for such settings. In order to get the colored results you have to set all the above mentioned properties to values that correspond to desired color space or you can initialize the TiffOptions structure with predefined settings as discussed ahead.

{{% /alert %}} 

Provided below is a table describing the expected parameter values that you can set in order to achieve desired results. Please note, you should set all 4 columns through TiffOptions in order to save any loaded/created image to TIFF file format.

|` `**TiffOptions.Photometric**|**TiffOptions.Compression**|**TiffOptions.BitsPerSample**|**TiffOptions.Predictor**|
| :- | :- | :- | :- |
|Palette|LZW/Uncompressed|1/4/8/16 (palette, color mode) single channel only|None|
|MinIsWhite/MinIsBlack|LZW/Uncompressed|1/4/8/16 (gray-scale mode) single channel only|None|
|Palette|LZW/Uncompressed|8 (palette, color mode) single channel only|Horizontal (more compression achieved for LZW same patterns)|
|MinIsWhite/MinIsBlack|LZW/Uncompressed|8 (gray-scale mode) single channel only|Horizontal (more compression achieved for LZW same patterns)|
|RGB|LZW/Uncompressed|[8,8,8] (3 RGB channels)|None/Horizontal|
|RGB|LZW/Uncompressed|[8,8,8,8] (3 RGB channels and additional alpha channel may be set through TiffOptions.AlphaStorage) Actually any additional channels count is supported but each channel must have 8 bit size like [8,8,8,8,8,8]|None/Horizontal|
All 4 properties should be set through TiffOptions in order to save any image format to Tiff format.

{{% alert color="primary" %}} 

When employing different combinations, some viewers (including the Windows Photo Viewer) may refuse to render the resultant image due to the limited support they offer. In such case, please pick different viewer for your testing.

{{% /alert %}} 
### **Predefined Settings for TiffOptions Class**
In order to facilitate the users and to avoid the miss-configuration of the TiffOptions instance, the Aspose.Imaging for Java API has exposed another constructor that accepts a parameter of type TiffExpectedFormat. Based on the selected value from the TiffExpectedFormat enumeration, the API auto configures all the mandatory properties for the TiffOptions instance in order to produce the desired results.

Before we move towards the sample code, here is the list of the TiffExpectedFormat fields and their details for better understanding of the usage.

1. TiffExpectedFormat.Default: Setting the field to Default acts similar to the default constructor of TiffOptions class with no compression set and BitsPerPixel set to 1 in order to produce a black n white result. It is advised to use this field when other format specific properties are to be set manually according to the desired results.
1. TiffExpectedFormat.TiffCcitRle: Specific to RLE encoding while saving the result in 1 BitsPerPixel (black n white) TIFF format.
1. TiffExpectedFormat.TiffCcittFax3: Specific to CCITT Fax3 encoding while saving the result in 1 BitsPerPixel (black n white) TIFF format.
1. TiffExpectedFormat.TiffCcittFax4: Specific to CCITT Fax4 encoding while saving the result in 1 BitsPerPixel (black n white) TIFF format.
1. TiffExpectedFormat.TiffDeflateBW: Specific to Deflate compression while saving the result in 1 BitsPerPixel (black n white) TIFF format.
1. TiffExpectedFormat.TiffDeflateRGB: Specific to Deflate compression while saving the result in RGB (color) TIFF format.
1. TiffExpectedFormat.TiffJpegRGB: Specific to Jpeg compression while saving the result in RGB (color) TIFF format.
1. TiffExpectedFormat.TiffJpegYCBCR: Specific to Deflate compression while saving the result in YCBCR (color) TIFF format.
1. TiffExpectedFormat.TiffLzwBW: Specific to LZW compression while saving the result in 1 BitsPerPixel (black n white) TIFF format.
1. TiffExpectedFormat.TiffLzwRGB: Specific to LZW compression while saving the result in RGB (color) TIFF format.
1. TiffExpectedFormat.TiffLzwRGBA: Specific to LZW compression while saving the result in RGBA (color with transparency) TIFF format.
1. TiffExpectedFormat.TiffNoCompressionBW: Specific to uncompressed TIFF format while saving the result in 1 BitsPerPixel (black n white).
1. TiffExpectedFormat.TiffNoCompressionRGB: Specific to uncompressed TIFF format while saving the result in RGB (color).
1. TiffExpectedFormat.TiffNoCompressionRGBA: Specific to uncompressed TIFF format while saving the result in RGBA (color with transparency).

The following code snippet elaborates the usage of TiffExpectedFormat fields while creating an instance of TiffOptions class.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingTIFFImages-TiffOptionsConfiguration-TiffOptionsConfiguration.java" >}}
## **Support for Deflate and Adobe Deflate Compression**
The TIFF (Tagged Image File Format) file format supports various types of compression whereas the compression type is stored as a tag (an integer value) in the file. One of such compression methods is Adobe Deflate (previously known as Deflate). Since the release of Aspose.Imaging for Java 2.8.0, the API supports this compression method for loading, converting & creating TIFF images.
### **Loading Image**
Aspose.Imaging for Java API hides all the ugly details from the user and provides an easy to use mechanism to load images for further processing. In order to load a TIFF image having Adobe Deflate compression, user has to pass the file path location or stream object to the Image.Load method and cast the object to [TiffImage](https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.tiff/tiffimage) as per requirement.
### **Support Tiff deflate Images with Alpha**
Aspose.Imaging for Java API hides all the ugly details from the user and provides an easy to use mechanism to load images for further processing. In order to load a TIFF image and save that with Deflate compression with Alpha, user has to pass the file path location or stream object to the Image.load method and cast the object to [TiffImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffImage) as per requirement.
### **Saving Image**
Converting any raster image to TIFF with Deflate/Adobe Deflate compression is easy as follow.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-SavingRasterImageToTIFFWithCompression.java" >}}

### **Creating Image**
Below provided sample demonstrates the usage of Aspose.Imaging for Java API to create an image from scrach using the Adobe Deflate compression method.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-CreatingTIFFImageWithCompression.java" >}}

## **Compressing TIFF Images**
Aspose.Imaging for Java API can be used to convert other raster formats to TIFF image format and even change the compression of existing TIFF image. The API can also be used to store different images as frames in a TIFF image for archiving purposes while compressing the images to lowest data size. The image compression in any case should be performed by reducing the source data size regardless of the compression algorithm used. In order to achieve the best compression ratio we may use indexed color spaces. The below provided code snippet performs the best compression using 16 indexed colors only and LZW compression algorithm however the source colors are slightly dithered.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-CompressingTIFFImagesWithLZWAlgorithm.java" >}}

Another approach which can be used since the release of Aspose.Imaging for Java v2.8.0 is by using the Adobe Deflate compression as demonstrated below.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-CompressingTIFFImagesWithAdobeDeflateCompression.java" >}}

## **Splitting TIFF Frames**
A Tiff image can have multiple frames and a requirement may arise to split these frames into several images. This article demonstrates the use of Aspose.Imaging for Java API to achieve this requirement in an efficient manner with a few lines of code.
### **Saving Each Frame in TIFF Format**
Splitting the Tiff frames is easy and can be achieved in below simple steps.

1. Firstly, create an instance of [TiffImage](https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff/TiffImage) and load a Tiff file from the disk/stream.
1. Iterate over the Tiff frame collection.
1. Save each frame to disc in Tiff format.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-SplittingTiffFrames.java" >}}


### **Saving Each Frame in Other Format**
Most of the process is the same as discussed above with a minor change, that is; while saving the frame to disc, you may pass an object of the ImageOptionBase according to the desired raster image format. Below provided code snippet demonstrates this concept by saving each frame in PNG format.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-SavingEachFrameInOtherRasterImageFormat.java" >}}

## **Memory strategy optimization**
Loading and saving of Tiff images can be proceeded using memory strategy optimization - ie limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "MemoryStrategyOptimizationTiff.java" >}}

## **Get tiff original options from image**
Aspose.Imaging Java API allows to save tiff images in original format keeping all original settings.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "get-tiff-original-options.java" >}}

## **Tiff image export in batch mode**
Aspose.Imaging library supports possibility of batch conversion before saving (exporting) Tiff images. This makes it possible not to keep in memory the resources of all processed pages at the same time, which will certainly give a significant performance boost with a lack of memory. With enough memory, the performance in standard mode and batch mode is the same, but the memory consumption in batch mode is much lower for multi-page tiff images (see illustrations below).

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Tiff-batch-mode-example.java" >}}

## **Export tiff to pdf (set dpi for exported pdf)**
Aspose.Imaging library supports possibility to convert image to pdf and specify DPI for exported pdf
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-set-dpi-in-exported-pdf.java" >}}

## **Support for extracting paths from TIFF**
#### **Clipping Path**
Clipping path is the Photoshop technique to remove the background from an image. Photoshop allows you to select a part of an image using Clipping Path and save the path within a file. Clipping Paths allow you to hide the part of an image you don't want to appear. Anything inside the clipping path will be visible, but anything outside of it will be transparent.

Other words Photoshop makes it possible to isolate certain parts of an image, without permanently changing the layer. This allows you to tweak the image at any point in the creative process. Clipping Paths are a traditional method of cutting out objects or people in Photoshop that allows you to create image files with transparent backgrounds. This approach works best with objects or people with "hard" edges around the object or person you want to cut out.
#### **Access Clipping Paths in TIFF image**
*PathResources* property allows you to access Clipping Paths in TIFF frame. The following code retrieves paths from TIFF image and displays their names in the console:

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Access-Clipping-Path-In-Tiff-Image.java" >}}
#### **Modify existing Clipping Paths**
You can easily modify already existing Clipping Paths. For instance, you can keep only one Clipping Path in the image:

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Modify-Clipping-Path-In-Tiff-Image.java" >}}
#### **Create Clipping Path manually**
You can manually create Clipping Path in TIFF image. In order to do that you need to create an instance of *PathResource* class. The following code demonstrates the way how you can create an empty path in TIFF image:

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-Create-Clipping-Path-Manually.java" >}}

#### **Get existing Clipping Path**
The following code shows how to get existing Clipping Path from TIFF image:
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-get-existing-clipping-path.java" >}}

#### **Change Clipping Path**
In case if you have multiple paths in TIFF image you can easily change which of them is Clipping Path:
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-change-clipping-path.java" >}}

#### **Create Clipping Path from scratch**
The following source code sample demonstrates how to create paths in TIFF image from scratch:
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-create-clipping-path-from-scratch.java" >}}

#### **Clipping Path content**
To create your own Clipping Paths you need to understand their content. Photoshop stores its paths as resources with IDs in the range 2000 through 2997. The name of the resource is the name given to the path when it was saved. If the file contains a resource with an ID of 2999, then this resource contains the name of the clipping path. Each path has a set of records to hold the data.

**Record classes:** 
*LengthRecord* - contains the number of Bezier knot records.
*BezierKnotRecord* - describes the knots of the path.
*ClipboardRecord* - contains four fixed-point numbers for the bounding rectangle.

More details you can find in [Adobe Photoshop File Formats Specification](https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/).
