---
title: Python and .NET Version Differences
second_title: Aspose.Imaging for Python via .NET
articleTitle: Python and .NET Version Differences
linktitle: Python and .NET Version Differences
description: "Aspose.Imaging for Python via .NET is a wrapper of Aspose.Imaging for .NET, this page describes the differences in features and API of these two products."
type: docs
weight: 15
url: /ru/python-net/python-notes/
aliases: [/python/python-notes/]
---

Aspose.Imaging for Python via .NET is a wrapper of Aspose.Imaging for .NET, that is why the two products have almost the same set of features. Nevertheless, there are some nuances of work and differences in features and API, which are described on this page.

## Feature Differences

Due to the wrapping process there are some features that are not available in the Python version. Here is a list of most notable features that are currently are not available in the Python version.<br>
**Implementation of interfaces is not supported yet, that is why it is not possible to use callbacks such as**

- [IPartialArgb32PixelLoader](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/ipartialargb32pixelloader/)
- [IPartialArgb64PixelLoader](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/ipartialargb64pixelloader/)
- [IImageLoader](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimageloader/)
- [IImageLoaderDescriptor](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimageloaderdescriptor/)
- [IImageExporter](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimageexporter/)
- [IImageExporterDescriptor](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimageexporterdescriptor/)
- [IImageCreator](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimagecreator/)
- [IImageCreatorDescriptor](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/iimagecreatordescriptor/)
- [IColorPalette](https://reference2.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging/icolorpalette/)
- and other interfaces and callbacks/delegates

## Casting Aspose.Imaging Objects in Python

Though type casting is not natural for Python developers some tasks cannot be accomplished without casting documents nodes or fields to concrete type. Aspose.Imaging for Python via .NET provides special methods that allow casting objects where this is necessary.

### Casting Images 
Base class for all formats of images in Aspose.Imaging is [Image](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/)

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

## Non-standard collections and features

Due to the fact that Aspose.Imaging for Python via .NET is based on .NET assembly, some properties and methods returns non-standard collections which are wrappers over the native .NET classes.

### Arrays

Actually returning arrays are classes that support standard access to their elements using `array[index]`, but they do not support the `len()` function. Instead, their size could be gotten using the property `length`.
**Supported methods/properties**
- Method `index()`
- Method `count()`
- Method `sort()`
- Method `reverse()`
- Method `copy()`
- Method `contains()`
- Iterator `__iter__`
- Property `length` 

``` python
pixels = image.load_argb_32_pixels(Rectangle(10, 10, 20, 20))
print("The length of pixels is", pixels.length) # can not be used `len(pixels)`
# or you can do like this
list_copy = list(pixels)
print("The length of list_copy is", len(list_copy)) 
```

Arrays might be converted into standard Python lists by calling `list(pixels)`, but it takes time and more memory to copy all elements.

### Lists
Returning list are classes that support the following methods. But they do not support the `len()` function. Instead, their size could be gotten using the property `length`.

**Supported methods/properties**
- Method `pop()`
- Method `index()`
- Method `count()`
- Method `sort()`
- Method `reverse()`
- Method `copy()`
- Method `append()`
- Method `remove()`
- Method `clear()`
- Method `contains()`
- Iterator `__iter__`
- Property `length` 

Lists might be converted into standard Python lists by calling `list()`, but it takes time and more memory to copy all elements.

## I/O Non-standard Classes
Aspose.Imaging presents the following methods for working with memory and files as with streams.

**Package: ** [aspose.imaging.extensions](https://reference.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging.extensions)

**Class: ** [StreamExtensions](https://reference.aspose.com/imaging/ru/python-net/api-reference/aspose.imaging.extensions/streamextensions/)

| Method | Description |
|--------|-------------|
| create_memory_stream() | Creates and returns the stream that is actually placed in the memory and automatically extends when something is written in it. |
| create_memory_stream_with_size(capacity) | The same with `create_memory_stream()` but the stream is already allocated with `capacity`. |
| create_memory_stream_from_bytes(array) | Wraps `array` and allows work with it as with a stream. |
| create_file_stream(path, file_mode) | Creates/opens a file in binary mode.<br> `path` is a path to a file.<br> `file_mode` can be one of the values of the enum **aspose.pyio.FileMode**.<br> - `FileMode.APPEND` - opens an existing file and appends data to the end of it.<br> - `FileMode.CREATE` - creates a new file or rewrites if it exists.<br> - `FileMode.CREATE_NEW` - creates a new file or throws an exception if it exists.<br> - `FileMode.OPEN` - opens file or throws exception if it does not exist.<br> - `FileMode.OPEN_OR_CREATE` - opens an existing file or creates if the file does not exist.<br> - `FileMode.TRUNCATE` - open an existing file and truncates it. |

### Using MemoryStream

``` python

from aspose.imaging.extensions import StreamExtensions as streams

with streams.create_memory_stream() as mem:
  image.save(mem) # here we save the image into memory like in a file
  
  mem.seek(0)
  first_bytes = mem.read(4)
  mem.seek(0)
  with Image.load(mem) as img2:
	# do something
	pass

```

### Using FileStream

``` python

from aspose.pyio import FileMode
from aspose.imaging.extensions import StreamExtensions as streams

with streams.create_file_stream('/tmp/outfile.bmp', FileMode.CREATE) as file_bmp:
  image.save(file_bmp) # export in the file
  
  file_bmp.seek(0)
  first_bytes = file_bmp.read(4)
  file_bmp.seek(0)
  with Image.load(file_bmp) as img2:
	# do something
	pass

```

## API Members Naming
To be closer to Python world, API members of Aspose.Imaging for Python via .NET uses a python snake style, however in most cases they have one to one analog in Aspose.Imaging for .NET API. You can find these analog in the [xml file](wrapper.zip).
