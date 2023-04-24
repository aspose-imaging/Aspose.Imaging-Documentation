---
title: Python and .NET Version Differences
second_title: Aspose.Imaging for Python via .NET
articleTitle: Python and .NET Version Differences
linktitle: Python and .NET Version Differences
description: "Aspose.Imaging for Python via .NET is a wrapper of Aspose.Imaging for .NET, this page describes the differences in features and API of these two products."
type: docs
weight: 15
url: /python-net/python-notes/
aliases: [/python/python-notes/]
---

Aspose.Imaging for Python via .NET is a wrapper of Aspose.Imaging for .NET, that is why the two products have almost the same set of features. Nevertheless, there are some nuances of work and differences in features and API, which are described on this page.

## Feature Differences

Due to the wrapping process there are some features that are not available in the Python version. Here is a list of most notable features that are currently are not available in the Python version.
* Implementation of interfaces is not supported yet, that is why it is not possible to use callbacks such as 
- [IPartialArgb32PixelLoader](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/ipartialargb32pixelloader/) \
- [IPartialArgb64PixelLoader](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/ipartialargb64pixelloader/) \
- [IImageLoader](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimageloader/) \
- [IImageLoaderDescriptor](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimageloaderdescriptor/) \
- [IImageExporter](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimageexporter/) \
- [IImageExporterDescriptor](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimageexporterdescriptor/) \
- [IImageCreator](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimagecreator/) \
- [IImageCreatorDescriptor](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/iimagecreatordescriptor/) \
- [IColorPalette](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/icolorpalette/)
- and other interfaces and callbacks/delegates

## Casting Aspose.Imaging Objects in Python

Though type casting is not natural for Python developers some tasks cannot be accomplished without casting documents nodes or fields to concrete type. Aspose.Imaging for Python via .NET provides special methods that allow casting objects where this is necessary.

### Casting Images 
Base class for all formats of images in Aspose.Imaging is [Image](https://reference2.aspose.com/imaging/python-net/api-reference/aspose.imaging/image/)

{{< highlight python >}}
from aspose.imaging import Image
from aspose.imaging.fileformats.jpeg import JpegImage
import aspose.pycore as casting
# always use image objects in `with..as..` for correct disposing
with Image.load("image.jpg") as image:
  # get the image format
  print(FileFormat(image.file_format))
  # but for accessing to the properties and methods which are specific for someone image format, we need to cast it to a necessary class by the following mode
  jpeg_image = casting.as_of(image, JpegImage)
  # now we have an access to some specific properties and methods of JpegImage
  print(jpeg_image.jfif) # access to JFIF data
  print(jpeg_image.exif_data) # access to EXIF data
  # and so on
{{< /highlight >}}


## Casing Functions of the package `aspose.pycore`
| Function   | Description |
|----------  | ----------- |
| cast&nbsp;(T,&nbsp;obj) | Casts or converts a wrapper-object **obj** to a type **T**.<br><br>The function returns a new wrapper-object of `T` created for the underlying .Net object of the Python object `obj`. If `obj` cannot be cast to `T`, an error occurs. Unlike the `as_of` function, this function converts `obj` to `T` with respect to internal methods possibly defined in `T` for explicit conversions between `T` and the original `obj` type.<br><br>**Parameters:**<ul><li>`T` - the target object type.</li><li>`obj` - any wrapper-object.</li></ul>**Returns:**<br> object translated to `T`|
| as_of(obj, T) | Reinterprets `obj` as an object of `T`<br>The function returns a new wrapper-object of `T` created for the underlying .Net object of the Python object `obj`. If `obj` cannot be cast to `T`, an error occurs. Unlike the `cast` function, this function converts `obj` to T without regard to internal methods possibly defined in `T` for explicit conversions between T and the original type of 'obj'.<br>**Parameters:**<ul><li>`obj` - any wrapper-object.</li> <li>`T` - the target object type.</li></ul>**Returns:**<br>object translated to `T`|
| is_assignable(obj, T) | Returns **True** if `obj` can be cast to `T` with the `as_of` function, otherwise **False**|
| is_typeof_eq&nbsp;(obj, T) | Returns **True** if the original wrapper-type of the underlying .Net object of the Python object `obj` is `T` otherwise **False**|
| type_of(T) | Returns a wrapper-object representing the underlying .Net type for  `T` |

## API Members Naming
To be closer to Python world, API members of Aspose.Imaging for Python via .NET uses a python snake style, however in most cases they have one to one analog in Aspose.Imaging for .NET API. You can find these analog in the [xml file](wrapper.zip).
