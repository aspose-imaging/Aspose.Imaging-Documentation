---
title: Creating, Opening and Saving Images
type: docs
weight: 40
url: /net/creating-opening-and-saving-images/
---

## **Creating Image Files**
Aspose.Imaging for .NET allows developers to create their own images. Use the static [Create](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/create) method exposed by the [Image](https://apireference.aspose.com/imaging/net/aspose.imaging/image) class to create new images. All you need to do is to supply the appropriate object of one of the classes from the [ImageOptions](/pages/createpage.action?spaceKey=imagingnet&title=Aspose.Imaging.ImageOptions+namespace&linkCreation=true&fromPageId=14779055) namespace for the desired output image format. To create an image file, first create an instance of one of the classes from the ImageOptions namespace. These classes determine output image format. Below are some classes from the [ImageOptions](/pages/createpage.action?spaceKey=imagingnet&title=Aspose.Imaging.ImageOptions+namespace&linkCreation=true&fromPageId=14779055) namespace:

- [BmpOptions]() sets the options for creating a BMP file
- [GifOptions]() sets the options for creating a GIF file
- [JpegOptions]() sets the options for creating a JPEG file
- [PngOptions]() sets the options for creating a PNG file
- [TiffOptions]() sets the options for creating a TIFF file
- [PsdOptions]() sets the options for creating a PSD file

Image files can be created [setting an output path](http://www.aspose.com/docs/display/imagingnet/Creating%2C+Opening+and+Saving+Images#Creating%2COpeningandSavingImages-CreatingbySettingPath) or by [setting a stream](http://www.aspose.com/docs/display/imagingnet/Creating%2C+Opening+and+Saving+Images#Creating%2COpeningandSavingImages-CreatingUsingStream).
### **Creating by Setting Path**
Create an object of any desired class from the [ImageOptions](https://apireference.aspose.com/imaging/net/aspose.imaging/imageoptionsbase) namespace and set the various properties. The most important property to set is the Source property. This property specifies where the image data resides (in a file or a stream). In the example below, the source is a file. After setting the properties, pass the object to one of the static Create methods along with width and height parameter.The width and height are defined in pixels. In the example below, we are creating a BMP file so we need to create an instance of ImageOptions.BmpOptions.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-DrawingAndFormattingImages-CreatingAnImageBySettingPath-CreatingAnImageBySettingPath.cs" >}}
### **Creating Using Stream**
The process for creating an image using a stream is same as for using a path. The only difference is that you need to create an instance of StreamSource by passing a Stream object to its constructor and assigning it to the Source property. The following code snippet shows you how to create Using Stream.

{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "Examples-CSharp-DrawingAndFormattingImages-CreatingImageUsingStream-CreatingImageUsingStream.cs" >}}
## **Opening Image Files**
Developers can use Aspose.Imaging for .NET API to open existing image files for different purposes, like adding effects to the image or to convert an existing file to another format. Whatever the purpose is, Aspose.Imaging provides two standard ways to open existing files: [from file](http://www.aspose.com/docs/display/imagingnet/Creating%2C+Opening+and+Saving+Images#Creating%2COpeningandSavingImages-OpeningfromDisk) or [from a stream](http://www.aspose.com/docs/display/imagingnet/Creating%2C+Opening+and+Saving+Images#Creating%2COpeningandSavingImages-OpeningusingaStream).
### **Opening from Disk**
Open an image file by passing the path and file name as a parameter to the static method [Load](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/load/index) exposed by the [Image](https://apireference.aspose.com/imaging/net/aspose.imaging/image) class. The following code snippet shows you how to open image files from disk.

{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "Examples-CSharp-DrawingAndFormattingImages-OpeningAnImageFileFromDisk-OpeningAnImageFileFromDisk.cs" >}}
### **Opening using a Stream**
Sometimes the image that we need to open is stored as a stream. In such cases, use the overloaded version of the [Load](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/load) method. This accepts a Stream object as an argument to open the image. The following code snippet shows you how to open image files using a stream.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-DrawingAndFormattingImages-OpeningImageUsingStream-OpeningImageUsingStream.cs" >}}


## **Saving Image Files**
Aspose.Imaging lets you create image files from scratch. It also provides the means to edit existing image files. Once the image is created or modified, the file is usually saved to disk. Aspose.Imaging provides you with methods for saving images to a [disk by specifying a path](https://docs.aspose.com/imaging/net/drawing-images/#DrawingandFormattingImages-SavingtoDisk) or [using a Stream object](https://docs.aspose.com/imaging/net/drawing-images/#DrawingandFormattingImages-SavingtoaStream).
### **Saving to Disk**
The [Image](https://apireference.aspose.com/imaging/net/aspose.imaging/image) class represents an image object, so this class provides all the tools needed to create, load and save an image file. Use the [Image](https://apireference.aspose.com/imaging/net/aspose.imaging/image) class [Save](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/save/index) method to save images. One overloaded version of the [Save](https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/save/index) method accepts the file location as a string. The following code snippet shows you how to save image files to disk.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-DrawingAndFormattingImages-SavingToDisk-SavingToDisk.cs" >}}


### **Saving to a Stream**
Another overloaded version of the [Save](https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/1) method accepts the Stream object as an argument and saves the image file to the stream. The following code snippet shows you how to save image files to disk using a stream.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-DrawingAndFormattingImages-SavingToStream-SavingToStream.cs" >}}


If the image is created by specifying any of the CreateOptions in the [Image](https://apireference.aspose.com/imaging/net/aspose.imaging/image/constructors/main) constructor, the image is automatically saved to the path or stream supplied during the initialization of the [Image]() class by calling the Save method that doesn't accept any parameter.

### **Save image file extension aware**
Using Aspose.Imaging file extension maps to appropriative image options if you did not specified them.
{{< gist "aspose-com-gists" "f4a2faa9c7d3a77f599173aee0927a3b" "save-image-file-extension-aware.cs" >}}

### **Setting for Replacing Missing Fonts**
Developers can use Aspose.Imaging for .NET API to load existing image files for different purposes and this default font should be used as a replacement for all missing fonts (fonts that are not found in current Operating System). Once the image is modified, the file is will be saved to disk.

{{< gist "aspose-imaging" "b93073a27bcdd4fefc2821e113f0cb3a" "Examples-CSharp-ModifyingAndConvertingImages-MetaFiles-SupportForReplacingMissingFonts-SupportForReplacingMissingFonts.cs" >}}
## **Image load/save indication progress**


{{< gist "aspose-com-gists" "2d1bcb9853315458808ffbcd9e7e3e02" "ProgressCallback.cs" >}}




