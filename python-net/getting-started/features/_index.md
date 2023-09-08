---
title: Features
second_title: Aspose.Imaging for Python via .NET
type: docs
weight: 30
url: /python-net/features/
description: Python image processing library core features includes read and write images, draw images, process images and convert between formats.
---

## **Supported Platforms**

The platforms Aspose.Imaging for Python via .NET can be used on Windows x64 and wide range of Linux distributions with Python 3.5 or later installed. There are additional requirements to the target Linux platform:

- GCC-6 runtime libraries (or later)
- Dependencies of .NET Core Runtime. Installing .NET Core Runtime itself is NOT required
- For Python 3.5-3.7: The pymalloc build of Python is needed. The --with-pymalloc Python build option is enabled by default. Typically, the pymalloc build of Python is marked with m suffix in the filename.
- libpython shared Python library. The --enable-shared Python build option is disabled by default, some Python distributions do not contain the libpython shared library. For some linux platforms, the libpython shared library can be installed using the package manager, for example: sudo apt-get install libpython3.7. The common issue is that libpython library is installed in a different location than the standard system location for shared libraries. The issue can be fixed by using the Python build options to set alternate library paths when compiling Python, or fixed by creating a symbolic link to the libpython library file in the system standard location for shared libraries. Typically, the libpython shared library file name is libpythonX.Ym.so.1.0 for Python 3.5-3.7, or libpythonX.Y.so.1.0 for Python 3.8 or later (for example: libpython3.7m.so.1.0, libpython3.9.so.1.0).

If you need support for more platforms, look for the “twin brother” products Aspose.Imaging for .NET or Aspose.Imaging for Java.

## **Product Features**
The following are Aspose.Imaging's core features:

- Read images
- Write images
- Draw images
- Process images
- Convert between formats

### **Feature List**
#### **Image Creations**
- Bmp
- Dicom
- Dxf
- Emf
- Emfz (Compressed Emf)
- Gif
- Html5
- Ico
- Jpeg (v2.3 now supports own codec)
- Jpeg2000 (v2.8)
- Apng (Animated PNG)
- Pdf
- Png (v2.5 now supports own codec)
- Psd (v2.7 added Jpeg thumbnails encoding/decoding support)
- Svg
- Svgz (Compressed Svg)
- Tga
- Tiff
- BigTiff
- WebP
- Wmf
- Wmfz (Compressed Wmf)
#### **Image Loading**
- Bmp
- Cdr
- Cmx
- Dib
- Dicom
- Djvu
- Dng
- Emf
- Eps
- Gif
- Ico
- Jpeg
- Jpeg2000 (v2.8)
- ODG
- OTG
- Apng (Animated PNG)
- Png
- Svg
- Tga
- Tiff
- BigTiff
- WebP
- Wmf
#### **Raw Data Processing**
- Bmp (v2.4, partly only raw data load)
- Gif
- Jpeg
- Jpeg2000
- Png
- Psd
- Tiff
- BigTiff
#### **Bmp Compression**
- Rle
#### **Psd Compressions**
- Rle
- Uncompressed
#### **Tiff Compressions**
- CCITT3
- CCITT4
- Rle
- Uncompressed
- Lzw
- Deflate (v2.6)
- Loading others (on below of GDI+)
- Jpeg (only 8 bps)
- Tiff color spaces
- RGB
- CMYK
- CIELAB
- YCrCb
#### **Tiff color spaces**
- RGB    
- CMYK (reading only) (v2.1)
- CIELAB (reading only) (v2.1)
- YCrCb    
#### **Drawing Features**
- Large images    
- Rotate    
- Flip    
- Scale    
- Cache system    
- Custom user images    
- SHA2 certificate (v2.0)
- Read/Write Exif data (v2.0)
- Tiff data recovery (v2.2)
- Dithering (v2.2)
- Dual sign (v2.3)
- Crop (v2.3)
- Vector to raster export    
- Brightness, contrast, gamma update (v2.6)
- Xmp data support
- Drawing and filling of basic shapes (Line, Polygon, Rectangle, Cubic Bézier, Curve, Arc, Ellipse, Pie, Path)
- Clear
- Clipping to rectangular region (Implemented clipping to image boundaries for existing drawing algorithms)
- Matrix transformations (Matrix transformations are implemented partially, mostly for internal needs of drawing engine)
#### **Image processing features**
- Image masking
- Image filters
- Image deskew
- Image resize
