---
title: What's New in Aspose.Imaging for .NET
type: docs
weight: 5
url: /net/what-s-new-in-aspose-imaging-for-net/
keywords: C# image library, C# image processing
description: C# image processing library supports most common raster file formats and offers a wide range of compression algorithms, image export and image conversion.
---

This page highlights the new features and enhancements introduced in recent releases of Aspose.Imaging graphic library.

## Aspose.Imaging for .NET 24.4

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Enhance your API capabilities with the latest update! Now you can effortlessly adjust Dicom tags via our public API, empowering seamless integration and customization. Experience improved PNG loading, including support for files with unexpected end of file (EOF), alongside optimized PNG loader performance. Convert DJVU files to PDF with ease, ensuring the first page is not blank. Plus, tackle EMF to PDF conversions effortlessly with text wrapping enhancements. We resolve issues with converting CDR images to DXF format. Enjoy smoother EPS to SVG exports with fixes for processing errors and missing text. Witness a significant performance boost in exporting large SVG files. Get ready for enhanced productivity with our latest PS (EPS) file export fixes. Upgrade now and streamline your workflow with precision and efficiency!
</p>

### New Feature - Edit DICOM Image Tags

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the most recent update, you now can modify DICOM image tags. You can achieve this by updating an existing tag using the UpdateTag() method, adding a new tag with AddTag(), or completely removing a tag using the RemoveTag() method. Below is a C# code example demonstrating how to load a DICOM image, edit its tags, and then save the edited output images.
</p>

```cs
using (DicomImage image = (DicomImage)Image.Load("ttfm.dcm"))
{
    image.FileInfo.UpdateTag("Patient's Name", "Test Patient");
    image.FileInfo.AddTag("Angular View Vector", 234);
    image.FileInfo.RemoveTag("Station Name");

    image.Save("output.dcm");
}
```

Please visit the <a href="https://releases.aspose.com/imaging/net/release-notes/2024/aspose-imaging-for-net-24-4-release-notes/">Aspose.Imaging 24.4 release notes</a> for more details.


## Aspose.Imaging for .NET 24.3

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Improve your document conversion experience with our latest enhancements! Our updated conversion system seamlessly transforms TIFF files with different horizontal and vertical resolutions into PDFs, ensuring precise preservation without distortion. Additionally, we've addressed unauthorized access exceptions encountered when loading read-only image files, guaranteeing a secure and uninterrupted workflow. Embrace these advancements today to optimize your document management processes.
</p>

For further details, please explore the <a href="https://releases.aspose.com/imaging/net/release-notes/2024/aspose-imaging-for-net-24-3-release-notes/">Aspose.Imaging 24.3 release notes</a>.

## Aspose.Imaging for .NET 24.2

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Maximize your productivity with our latest release. Harness the power of kernel filters with our enhanced support, delivering stunning image and photo effects capabilities. Seamlessly integrate VSIX files into your workflow with improved recognition as SVG images. Addressing conversion challenges, we've resolved errors encountered when converting EPS images to PDF, ensuring a seamless transition. Additionally, we've tackled export issues with EPS to JPG conversions, guaranteeing faultless output quality. Experience enhanced efficiency as MSO files are now accurately recognized as SVG images. Moreover, streamline your memory usage during vector format rendering with our optimized processes. With precise step-by-step loading and rendering of each record, encounter no obstacles in your workflow. Embrace these advancements today and elevate your document management experience to new heights.
</p>

### New Feature - Kernel Filters Support

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Kernel filters are essential for image processing, offering a plethora of effects like Blur, Emboss, Gaussian Blur, and more. Aspose.Imaging for .NET goes beyond standard filters, enabling the creation of custom ones for unique image effects. These filters utilize a matrix called a "kernel" to manipulate pixels in the source image, applying the kernel matrix to each pixel through a mathematical convolution operation. Comprehensive code snippets featuring filter applications and accompanied by image examples can be found in our Developers Guide: <a href="/imaging/net/developer-guide/manipulating-images/kernel-filters/">Kernel Filters for Image Processing</a> article.
</p>

For additional details, explore the <a href="https://releases.aspose.com/imaging/net/release-notes/2024/aspose-imaging-for-net-24-2-release-notes/">Aspose.Imaging 24.2 release notes</a>.
