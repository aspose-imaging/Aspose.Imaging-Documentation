---
title: Manipulating EPS Images
type: docs
weight: 60
url: /net/developer-guide/manipulating-images/manipulating-eps-images/
description: Aspose.Imaging graphic library for .NET (C#) supports manipulating EPS images, exporting to other formats, resizing images and extracting preview images.
keywords: [vector graphics, eps images, export eps, convert eps, extract eps preview, export eps preview, preview image, eps to pdf]
---

## Export EPS images to other formats

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Encapsulated Postscript file (<a href="https://docs.fileformat.com/page-description-language/eps/">EPS</a>) is a vector graphics format with a history dating back to the 1980s. Even today, EPS remains a popular choice for combining text, graphics, and images, and it can be edited using vector graphic editor programs. The Aspose.Imaging graphic library offers methods to programmatically manipulate EPS images and export them to various standard image formats, such as JPG, PNG, SVG, TIFF, PSD or PDF.

In the C# code example below, we demonstrate how to load an EPS file and save it in SVG and PNG formats. When saving in PNG format, we utilize an additional option `PngColorType.Grayscale` to set the Grayscale palette:
</p>

{{< gist "aspose-com-gists" "6e07233cee28228d390f9d89418ac72d" "export-eps-to-other-format.cs" >}}

When converting EPS to PDF, you can set the required PDF compliance using the `PdfComplianceVersion.PdfA1b` option:

{{< gist "aspose-com-gists" "26c59ccd53d0f51adc9260323ff84979" "convert-eps-to-pdf.cs" >}}

## Resize EPS images before export

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Before converting the EPS image to another format, you have the flexibility to perform various manipulations. For instance, you can resize the image to larger dimensions by doubling the original width and height values:
</p>

{{< gist "aspose-com-gists" "6e07233cee28228d390f9d89418ac72d" "resize-and-export-eps.cs" >}}

## Extract preview image from the EPS files

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
EPS files usually contain a low-resolution preview image in black and white, which is compatible with various operating systems and can be rendered by most graphic applications. With the Aspose.Imaging library, you can extract the preview image and save it as a separate image file. In the example below, we use the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.eps/epsimage/getpreviewimage/">EpsImage.GetPreviewImage method</a> to obtain the existing preview image in a specific format. In our case, the preview is in TIFF format, and you can also get the preview image in WMF or JPEG formats using the appropriate values from the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.eps/epspreviewformat/">EpsPreviewFormat</a> enumeration:
</p>

{{< gist "aspose-com-gists" "6e07233cee28228d390f9d89418ac72d" "export-specific-eps-preview.cs" >}}
