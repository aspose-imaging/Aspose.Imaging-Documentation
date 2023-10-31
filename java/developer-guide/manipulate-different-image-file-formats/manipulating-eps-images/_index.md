---
title: Manipulating EPS Images
type: docs
weight: 60
url: /java/developer-guide/manipulating-images/manipulating-eps-images/
description: Aspose.Imaging graphic library for Java supports manipulating EPS images, exporting to other formats, resizing images and extracting preview images.
keywords: [Encapsulated Postscript, graphic library for Java, EPS images, export EPS, convert EPS, extract EPS preview, export eps preview, EPS to PDF, resize EPS]
---

## Export EPS images to other formats

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
PostScript documents have been adopted for combining text, graphics, and images into graphic files since the 1980s. The combined data is saved in the Encapsulated Postscript format (<a href="https://docs.fileformat.com/page-description-language/eps/">EPS</a>). EPS files are supported by many vector editing applications and remain popular for creating graphic documents. With the Aspose.Imaging graphic library for Java, you can rapidly develop applications or services to manipulate EPS images. You can easily load EPS files and convert them into other image vector or raster formats such as SVG, PNG, PDF, or PSD. In the Java code example provided, we export EPS images to SVG and PNG formats by using the `Save` method on the loaded EPS image object. For converting to the PNG format, we specify `PngColorType.Grayscale` as an additional option for a Grayscale PNG palette.
</p>

{{< gist "aspose-com-gists" "b3691dae7cbfae29eda2e3c45d75c514" "export-eps-to-other-format.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To export the loaded EPS image to a PDF document, utilize the option parameter `pdfCoreOptions` and specify the required PDF compliance version, such as `PdfA1b`, when saving the PDF file:
</p>

{{< gist "aspose-com-gists" "837f145431b5f9d11df9180e888451e7" "convert-eps-to-pdf.java" >}}

## Resize EPS images before export

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
When working with EPS images, you can perform various operations, such as resizing before exporting to another file format. Apply the `Resize` method to the loaded EPS image object to change the image width and height:
</p>

{{< gist "aspose-com-gists" "b3691dae7cbfae29eda2e3c45d75c514" "resize-and-export-eps.java" >}}

## Extract preview image from the EPS files

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Typically, EPS files also contain a low-resolution image preview embedded in the document, enabling other applications to display it. The preview can be stored in various formats within the file. To extract and save the preview image in TIFF, WMF, or JPEG format from an EPS file, utilize the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.fileformats.eps/epspreviewformat/">EpsPreviewFormat parameter</a> with the with <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.fileformats.eps/epsimage/#getPreviewImages--">getPreviewImages() method</a>:
</p>

{{< gist "aspose-com-gists" "b3691dae7cbfae29eda2e3c45d75c514" "export-specific-eps-preview.java" >}}
