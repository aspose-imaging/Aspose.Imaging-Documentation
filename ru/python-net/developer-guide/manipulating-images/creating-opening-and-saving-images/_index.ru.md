---
title: Creating, Opening and Saving Images
type: docs
weight: 40
url: /ru/python-net/creating-opening-and-saving-images/
---

## **Creating Image Files**
Aspose.Imaging for Python via .NET allows developers to create their own images. Use the static **Create** method exposed by the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class to create new images. All you need to do is to supply the appropriate object of one of the classes from the [ImageOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions) namespace for the desired output image format. To create an image file, first create an instance of one of the classes from the ImageOptions namespace. These classes determine output image format. Below are some classes from the [ImageOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions) namespace:

- [BmpOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.bmpoptions) sets the options for creating a BMP file
- [GifOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.gifoptions) sets the options for creating a GIF file
- [JpegOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.jpegoptions) sets the options for creating a JPEG file
- [PngOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.pngoptions) sets the options for creating a PNG file
- [TiffOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.tiffoptions) sets the options for creating a TIFF file
- [PsdOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions.psdoptions) sets the options for creating a PSD file

Image files can be created [setting an output path](#Creating%2COpeningandSavingImages-CreatingbySettingPath) or by [setting a stream](#Creating%2COpeningandSavingImages-CreatingUsingStream).

### **Creating by Setting Path**
Create an object of any desired class from the [ImageOptions](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.imageoptions/) namespace and set the various properties. The most important property to set is the Source property. This property specifies where the image data resides (in a file or a stream). In the example below, the source is a file. After setting the properties, pass the object to one of the static Create methods along with width and height parameter.The width and height are defined in pixels. In the example below, we are creating a BMP file so we need to create an instance of ImageOptions.BmpOptions.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "creating-image-by-setting-path.py" >}}

### **Creating Using Stream**
The process for creating an image using a stream is same as for using a path. The only difference is that you need to create an instance of StreamSource by passing a Stream object to its constructor and assigning it to the Source property. The following code snippet shows you how to create Using Stream.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "creating-image-using-stream.py" >}}

## **Opening Image Files**
Developers can use Aspose.Imaging for Python via .NET API to open existing image files for different purposes, like adding effects to the image or to convert an existing file to another format. Whatever the purpose is, Aspose.Imaging provides two standard ways to open existing files: [from file](#Creating%2COpeningandSavingImages-OpeningfromDisk) or [from a stream](#Creating%2COpeningandSavingImages-OpeningusingaStream).

### **Opening from Disk**
Open an image file by passing the path and file name as a parameter to the static method [load](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) exposed by the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class. The following code snippet shows you how to open image files from disk.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "opening-image-from-disk.py" >}}

### **Opening using a Stream**
Sometimes the image that we need to open is stored as a stream. In such cases, use the overloaded version of the [load](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) method. This accepts a Stream object as an argument to open the image. The following code snippet shows you how to open image files using a stream.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "opening-image-from-stream.py" >}}

## **Saving Image Files**
Aspose.Imaging lets you create image files from scratch. It also provides the means to edit existing image files. Once the image is created or modified, the file is usually saved to disk. Aspose.Imaging provides you with methods for saving images to a [disk by specifying a path](#DrawingandFormattingImages-SavingtoDisk) or [using a Stream object](#DrawingandFormattingImages-SavingtoaStream).

### **Saving to Disk**
The [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class represents an image object, so this class provides all the tools needed to create, load and save an image file. Use the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image) class [save](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) method to save images. One overloaded version of the [save](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) method accepts the file location as a string. The following code snippet shows you how to save image files to disk.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "saving-image-to-disk.py" >}}

### **Saving to a Stream**
Another overloaded version of the [Save](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.datastreamsupporter/save/methods/1) method accepts the Stream object as an argument and saves the image file to the stream. The following code snippet shows you how to save image files to disk using a stream.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "saving-image-to-stream.py" >}}

If the image is created by specifying any of the CreateOptions in the [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/) constructor, the image is automatically saved to the path or stream supplied during the initialization of the [Image]() class by calling the Save method that doesn't accept any parameter.

### **Save image file extension aware**
Using Aspose.Imaging file extension maps to appropriate image options if you did not specified them.
{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "save-image-file-extension-aware.py" >}}

### **Setting for Replacing Missing Fonts**
Developers can use Aspose.Imaging for Python via .NET API to load existing image files for different purposes and this default font should be used as a replacement for all missing fonts (fonts that are not found in current Operating System). Once the image is modified, the file is will be saved to disk.

{{< gist "aspose-com-gists" "8997090ce2d3e626fdc759cba091461e" "support-for-replacing-missed-fonts.py" >}}
