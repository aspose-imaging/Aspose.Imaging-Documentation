---
title: Manipulating TIFF Images
type: docs
weight: 160
url: /python-net/manipulating-tiff-images/
---

## **Add Frames with Different Settings**
TIFF is a very flexible format and it allows different frames to be added, with different dimensions, compression and other settings. Aspose.Imaging APIs allow you to add any TIFF frame of any size which helps in creating complex documents. If there is a requirement to adjust the frames during the add process to make them all equal, perform the following steps:

1. Create a new blank frame with the desired options or copy the source frame with the output options specified using the [create_frame_from](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe/) method.
1. Resize the source frame/image to the desired dimensions using the Resize method.
1. Add the source frame/image pixels to the new frame.
1. Add the new frame to the output TIFF image.

## **Export Multi Page frames to different Image format**
Sometimes you need to export Multi-page TIFF frames to some other image file format. This article will demonstrate how we can perform this task using Aspose.Imaging for Python via .NET API. We will use [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage), [TiffFrame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe), BmpOptions and BmpImage classes to export TIFF frames to BMP image format. First, we will create instance of TIFF image and load images from local disk. Now we will iterate over TIFF frames and copy pixels of active frame using [load_pixels](https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/) method into Colors array and create an instance of BmpOptions for BMP image settings. Set the desired setting for BMP image creation. Create a new BMP image using BmpOptions object and save BMP image using frame pixels, copied in Colors array.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "export-multipage-tiff-frames-to-another-format.py" >}}

Please note, the above provided code snippet requires setting the valid license for Aspose.Imaging for Python via .NET API. This is because Aspose.Imaging APIs restrict the usage of core features such as [load_pixels](https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/) & [save_pixels](https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/) in evaluation mode. Please check the details for [Evaluation Version Limitations_imaging.net]().

## **Adding Multiple images inside Tiff Frames**
` `This article will demonstrate how we can we add multiple images inside single tiff using Aspose.Imaging for Python via .NET API. We will use [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage), [TiffFrame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe),  classes to add multiple images inside tiff frames. Below provided code snippet demonstrates this concept.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "add-multiple-images-inside-tiff-frame.py" >}}

## **Concatenate Multiple TIFF Images**
Sometimes you need to concatenate a TIFF Image into another TIFF image to meet an application need. Aspose.Imaging APIs support the feature of concatenating multiple Tiff images, whereas this article exhibits the TIFF image concatenation feature of Aspose.Imaging for Python via .NET API. We will use [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage) and [TiffFrame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe) classes to concatenate multiple TIFF images. We can use both standard methods, from file and from stream, to concatenate TIFF images.

### **Images Having Single Frame**
{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "concatenate-multiple-tiff-images.py" >}}

#### **Concatenating Images from Disk**
Firstly, we will create instances of images and load images from the local disk, then we will copy the active frame of source image using [copy_frame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe/) method of [TiffFrame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffframe) class and add that copied frame to destination image with the help of [add_frame](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage/) method of [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage) class. Finally we will save image back to local disk.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "concatenate-multiple-tiff-images.py" >}}

#### **Concatenating Images from Stream**
Sometimes the images that we need to process are stored as a stream. In that case, use the overloaded version of the load method. Remaining logic would be remained same as described above.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "concatenate-multiple-tiff-images.py" >}}

### **Images Having Several Frames**
Below provided sample demonstrates the usage of Aspose.Imaging for Python via .NET API to concatenate Tiff images that could have several frames. For demonstration purposes, we will read a list of Tiff images, and create a new Tiff image that will hold the frames from all read Tiff images.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "concatenate-tiff-images-having-several-frames.py" >}}

## **Data Recovery Options**
Sometimes you may encounter a TIFF image that cannot be rendered properly while using traditional image viewers such as Windows Photo Viewer because the image is damaged or corrupted. When loaded with Aspose.Imaging, such images may throw exceptions and you may not be able to process them further. Aspose.Imaging 2.2.0 and later supports data recovery mode for TIFF files. The data recovery allows you to load a TIFF file that has improper data layout or corrupted data strips. Data recovery replaces the corrupted data with any color specified, and you can retrieve the rest of the data for further processing without experiencing any exception. This mechanism is especially useful for Tiff file format since it stores the data in strips. When a strip is damaged the other strips may still retain the correct information.

Aspose.Imaging provides two recovery modes which provide different results.

1. [CONSISTENT_RECOVER](https://reference.aspose.com/imaging/python-net/aspose.imaging/datarecoverymode): The consistent recovery mode tries to recover all data as long as corruption does not break the file format and allows further processing.
1. [MAXIMAL_RECOVER](https://reference.aspose.com/imaging/python-net/aspose.imaging/datarecoverymode): The maximal recovery mode recovers all data even if the file format has a corrupted structure and further processing may yield unexpected effects.

Below is sample code that shows how to use the two data recovery modes.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "tiff-data-recovery.py" >}}

When a damaged or corrupted TIFF file is loaded or saved without using data recovery you may get an exception.

## **TiffOptions Configuration**
Developers can adjust different properties of [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) class to get desired results. In this document, we will focus on 4 main properties that controls the resultant image attributes.

These properties are listed below.

1. [TiffOptions.photometric](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions)
1. [TiffOptions.compression](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions/)
1. [TiffOptions.bits_per_sample](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions/)
1. [TiffOptions.predictor](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions/)

Whenever we initialize an empty [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) structure, each option is set to its default value, for instance compression is set to None, bits_per_sample is set as 1 and photometric as MIN_IS_WHITE. Saving into this format will make the final image black n white and this is expected behavior for such options combination. In order to get the colored results you have to set all the above mentioned properties to values that correspond to desired color space or you can initialize the [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) structure with predefined settings as discussed later in this article. Provided below is a table describing the expected parameter values that you can set in order to achieve desired results. Please note, you should set all 4 columns through [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) in order to save any loaded/created image to TIFF file format.

|` `**TiffOptions.photometric**|**TiffOptions.compression**|**TiffOptions.bits_per_sample**|**TiffOptions.predictor**|
| :- | :- | :- | :- |
|Palette|LZW/Uncompressed|1/4/8/16 (palette, color mode) single channel only|None|
|MinIsWhite/MinIsBlack|LZW/Uncompressed|1/4/8/16 (gray-scale mode) single channel only|None|
|Palette|LZW/Uncompressed|8 (palette, color mode) single channel only|Horizontal (more compression achieved for LZW same patterns)|
|MinIsWhite/MinIsBlack|LZW/Uncompressed|8 (gray-scale mode) single channel only|Horizontal (more compression achieved for LZW same patterns)|
|RGB|LZW/Uncompressed|[8,8,8] (3 RGB channels)|None/Horizontal|
|RGB|LZW/Uncompressed|[8,8,8,8] (3 RGB channels and additional alpha channel may be set through TiffOptions.AlphaStorage) Actually any additional channels count is supported but each channel must have 8 bit size like [8,8,8,8,8,8]|None/Horizontal|

All 4 properties should be set through TiffOptions in order to save any image format to Tiff format. When employing different combinations, some viewers (including the Windows Photo Viewer) may refuse to render the resultant image due to the limited support they offer. In such case, please pick different viewer for your testing.

### **Predefined Settings for TiffOptions Class**
In order to facilitate the users and to avoid the miss-configuration of the [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) instance, the Aspose.Imaging for Python via .NET API has exposed another constructor that accepts a parameter of type TiffExpectedFormat. Based on the selected value from the TiffExpectedFormat enumeration, the API auto configures all the mandatory properties for the [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) instance in order to produce the desired results. Before we move towards the sample code, here is the list of the TiffExpectedFormat fields and their details for better understanding of the usage.

1. TiffExpectedFormat.Default: Setting the field to Default acts similar to the default constructor of [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) class with no compression set and BitsPerPixel set to 1 in order to produce a black n white result. It is advised to use this field when other format specific properties are to be set manually according to the desired results.
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

The following code snippet elaborates the usage of TiffExpectedFormat fields while creating an instance of [TiffOptions](https://reference.aspose.com/imaging/python-net/aspose.imaging.imageoptions/tiffoptions) class.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "tiff-options-configuration.py" >}}

## **Support for Deflate and Adobe Deflate Compression**
The TIFF (Tagged Image File Format) file format supports various types of compression whereas the compression type is stored as a tag (an integer value) in the file. One of such compression methods is Adobe Deflate (previously known as Deflate). Since the release of Aspose.Imaging 2.6.0, the API supports this compression method for loading, converting & creating TIFF images.

### **Loading Image**
Aspose.Imaging for Python via .NET API hides all the ugly details from the user and provides an easy to use mechanism to load images for further processing. In order to load a TIFF image having Adobe Deflate compression, user has to pass the file path location or stream object to the Image.Load method and cast the object to [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage) as per requirement.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "save-raster-image-to-tiff-with-compression.py" >}}

### **Support Tiff deflate Images with Alpha**
Aspose.Imaging for Python via .NET API hides all the ugly details from the user and provides an easy to use mechanism to load images for further processing. In order to load a TIFF image and save that with Deflate compression with Alpha, user has to pass the file path location or stream object to the Image.Load method and cast the object to [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage) as per requirement.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "save-raster-image-to-tiff-with-compression.py" >}}

### **Saving Image**
Converting any raster image to TIFF with Deflate/Adobe Deflate compression is easy as follow.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "save-raster-image-to-tiff-with-compression.py" >}}

### **Creating Image**
Below provided sample demonstrates the usage of Aspose.Imaging for Python via .NET API to create an image from scrach using the Adobe Deflate compression method.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "create-tiff-image-with-compression.py" >}}

## **Compressing TIFF Images**
Aspose.Imaging for Python via .NET API can be used to convert other raster formats to TIFF image format and even change the compression of existing TIFF image. The API can also be used to store different images as frames in a TIFF image for archiving purposes while compressing the images to lowest data size. The image compression in any case should be performed by reducing the source data size regardless of the compression algorithm used. In order to achieve the best compression ratio we may use indexed color spaces. The below provided code snippet performs the best compression using 16 indexed colors only and LZW compression algorithm however the source colors are slightly dithered.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "compressing-tiff-images-with-lzw-algorithm.py" >}}

Another approach which can be used since the release of Aspose.Imaging v2.6.0 is by using the Adobe Deflate compression as demonstrated below.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "compressing-tiff-with-adobe-deflate-compression.py" >}}

## **Splitting TIFF Frames**
A Tiff image can have multiple frames and a requirement may arise to split these frames into several images. This article demonstrates the use of Aspose.Imaging for Python via .NET API to achieve this requirement in an efficient manner with a few lines of code.

### **Saving Each Frame in TIFF Format**
Splitting the Tiff frames is easy and can be achieved in below simple steps.

1. Firstly, create an instance of [TiffImage](https://reference.aspose.com/imaging/python-net/aspose.imaging.fileformats.tiff/tiffimage) and load a Tiff file from the disk/stream.
1. Iterate over the Tiff frame collection.
1. Save each frame to disc in Tiff format.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "splitting-tiff-frames.py" >}}

### **Saving Each Frame in Other Format**
Most of the process is the same as discussed above with a minor change, that is; while saving the frame to disc, you may pass an object of the ImageOptionBase according to the desired raster image format. Below provided code snippet demonstrates this concept by saving each frame in PNG format.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "save-each-frame-in-other-raster-image-format.py" >}}

## **Memory strategy optimization**
Loading of Tiff images can be proceeded using memory strategy optimization - i.e. limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "memory-strategy-optimization-tiff.py" >}}

## **Get tiff original options from image**
Aspose.Imaging API allows to save tiff images in original format keeping all original settings.

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "get-tiff-original-options.py" >}}

## **Export tiff to pdf (set dpi for exported pdf)**
Aspose.Imaging library supports possibility to convert image to pdf and specify DPI for exported pdf
{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "tiff-export-to-pdf-set-dpi-in-pdf.py" >}}

## **Support for extracting paths from TIFF**
#### **Clipping Path**
Clipping path is the Photoshop technique to remove the background from an image. Photoshop allows you to select a part of an image using Clipping Path and save the path within a file. Clipping Paths allow you to hide the part of an image you don't want to appear. Anything inside the clipping path will be visible, but anything outside of it will be transparent.

Other words Photoshop makes it possible to isolate certain parts of an image, without permanently changing the layer. This allows you to tweak the image at any point in the creative process. Clipping Paths are a traditional method of cutting out objects or people in Photoshop that allows you to create image files with transparent backgrounds. This approach works best with objects or people with "hard" edges around the object or person you want to cut out.

#### **Access Clipping Paths in TIFF image**
*PathResources* property allows you to access Clipping Paths in TIFF frame. The following code retrieves paths from TIFF image and displays their names in the console:

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "access-clipping-path-in-tiff-images.py" >}}

#### **Modify existing Clipping Paths**
You can easily modify already existing Clipping Paths. For instance, you can keep only one Clipping Path in the image:

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "modify-clipping-path-in-tiff-images.py" >}}

#### **Create Clipping Path manually**
You can manually create Clipping Path in TIFF image. In order to do that you need to create an instance of *PathResource* class. The following code demonstrates the way how you can create an empty path in TIFF image:

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "create-clipping-path-in-tiff-manually.py" >}}

#### **Get existing Clipping Path**
The following code shows how to get existing Clipping Path from TIFF image:
{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "get-existing-tiff-clipping-path.py" >}}

#### **Change Clipping Path**
In case if you have multiple paths in TIFF image you can easily change which of them is Clipping Path:
{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "change-tiff-clipping-path.py" >}}

#### **Create Clipping Path from scratch**
The following source code sample demonstrates how to create paths in TIFF image from scratch:
{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "create-clipping-path-from-scratch.py" >}}

#### **Clipping Path content**
To create your own Clipping Paths you need to understand their content. Photoshop stores its paths as resources with IDs in the range 2000 through 2997. The name of the resource is the name given to the path when it was saved. If the file contains a resource with an ID of 2999, then this resource contains the name of the clipping path. Each path has a set of records to hold the data.

**Record classes:** 
*LengthRecord* - contains the number of Bezier knot records.
*BezierKnotRecord* - describes the knots of the path.
*ClipboardRecord* - contains four fixed-point numbers for the bounding rectangle.

More details you can find in [Adobe Photoshop File Formats Specification](https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/).
