---
title: Manipulating EPS Images
type: docs
weight: 60
url: /ru/python-net/developer-guide/manipulating-images/manipulating-eps-images/
description: Aspose.Imaging graphic library for Python supports manipulating EPS images, exporting to other formats, resizing images and extracting preview images.
keywords: [graphic library for Python, Encapsulated Postscript, EPS images, export EPS, convert EPS, extract EPS preview, export EPS preview, EPS embedded image]
---

## Export EPS images to other formats

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
One of the popular vector image formats for combining text, graphics, and images is Encapsulated Postscript (<a href="https://docs.fileformat.com/page-description-language/eps/">EPS</a>). EPS documents contain a PostScript program with page descriptions for publishing and may also include encapsulated preview images. Vector graphic editing applications have used the EPS format to save graphic documents since the 1980s, and it continues to be widely used.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the Aspose.Imaging graphic library for Python, you can easily export EPS images to various file formats. To convert EPS images to other image formats, you simply load the EPS file into an `Image` object and save it in a different format, such as SVG, PNG, or PDF. Some image formats support various options for saving. In the case of the PNG image format, you can specify the color type as `PngColorType.GRAYSCALE`, as demonstrated in the Python code example below:
</p>

{{< gist "aspose-com-gists" "e9228688e0d1119d4e41cf361d646af0" "export-eps-to-other-format.py" >}}

## Resize EPS images before export

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Moreover, you can perform additional operations on the image before exporting it to another image format. For instance, you can resize the image by increasing its width and height:
</p>

{{< gist "aspose-com-gists" "e9228688e0d1119d4e41cf361d646af0" "resize-and-export-eps.py" >}}

## Extract preview image from the EPS files

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Some EPS files may contain embedded preview images for display in various graphic applications. These preview images can be in different formats like TIFF bitmap, Windows Metafile (WMF), or JPEG. Supported formats are listed in the <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.fileformats.eps/epspreviewformat/">EpsPreviewFormat Enumeration</a>. You can extract a preview image from the EPS file using the <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging.fileformats.eps/epsimage/#get_embedded_images__13">get_embedded_images() method</a> and save it as a separate file:
</p>

{{< gist "aspose-com-gists" "e9228688e0d1119d4e41cf361d646af0" "export-specific-eps-preview.py" >}}
