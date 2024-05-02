---
title: Manipulating Metafiles
type: docs
weight: 120
url: /ru/python-net/manipulating-metafiles/
---

## **Converting EMF To PDF**
Using Aspose.Imaging for Python via .NET, developers can convert EMF metafile to PDF format. This topic explains the approach to load existing metafiles and convert it to PDF. Aspose.Imaging for Python via .NET provides the **EmfImage** class to load EMF files and same can be used to save the image to PDF format. Below provided sample code demonstrate how to convert EMF to PDF.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "convert-emf-to-pdf.py" >}}

## **Cropping EMF Image**
**Image cropping** usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used to cut out some portion of an image to increase the focus on a particular area. Aspose.Imaging for Python via .NET API supports two different approaches for cropping image: by [shifts](https://docs.aspose.com/imaging/ru/python-net/manipulating-metafiles/#ManipulatingMetafiles-UsingShifts) and by [rectangle](https://docs.aspose.com/imaging/ru/python-net/manipulating-metafiles/#ManipulatingMetafiles-UsingRectangle).

#### **Using Shifts**
The EmfImage class provides an overloaded version of the [Crop](https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/) method that accepts 4 integer values denoting Left, Right, Top & Bottom. Based on these four values, the crop method moves the image boundaries toward the center of the image while discarding the outer portion.

The code snippet below demonstrates how to crop an EMF image by shifts.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "crop-emf-image.py" >}}


#### **Using Rectangle**
The EmfImage class provides another overloaded version of the crop method that accepts an instance of the Rectangle class. You can cut out any portion of an image by providing the desired boundaries to the Rectangle object. The code snippet below demonstrates how.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "crop-emf-image.py" >}}


## **Export MetaFile To Raster Formats**
Using Aspose.Imaging for Python via .NET, developers can convert metafile (Emf/Emf+) to raster formats. This article shows how to export/convert metafile file to raster image formats with Aspose.Imaging. Aspose.Imaging for Python via .NET provides the **EmfImage** class to load EMF files and same can be used to convert the Emf to raster formats. Below provided sample code demonstrate how to convert Emf/Emf+ to raster images.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "export-metafiles-to-raster-formats.py" >}}


## **Specifying Font Folder While Converting**
Using Aspose.Imaging for Python via .NET, developers can specify the font folder path used while converting WMF file. This topic explains the approach to specify the font folder that should be used. The following code snippet demonstrates the usage of Aspose.Imaging for Python via .NET API to change the font while converting EMF to raster image.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "specify-font-folder.py" >}}
## **Support For Replacing Missing Fonts**
Using Aspose.Imaging for Python via .NET, developers can replace missing fonts when saving ODG, SVG and MetaFile images. This topic explains the approach to replace the fonts that should be used. The following code snippet demonstrates the usage of Aspose.Imaging for Python via .NET API to replace the font while saving ODG images.

{{< gist "aspose-com-gists" "1c649f750396bf5e3444155268b7b727" "specify-font-folder.py" >}}
