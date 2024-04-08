---
title: What's New in Aspose.Imaging for .NET
type: docs
weight: 5
url: /net/what-s-new-in-aspose-imaging-for-net/
keywords: C# image library, C# image processing
description: C# image processing library supports most common raster file formats and offers a wide range of compression algorithms, image export and image conversion.
---

{{% alert color="primary" %}}

This page highlights the new features and enhancements introduced in recent releases of Aspose.Imaging graphic library. Your feedback is invaluable to us as we strive to improve our product. We greatly appreciate it if you take a moment to provide your insights on different aspects and complete the <a href="https://forms.gle/LRjHCzSrjfiqrkPQ6">Aspose.Imaging for .NET feedback form</a>.

{{% /alert %}}

## Aspose.Imaging for .NET 24.4

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Enhance your API capabilities with the latest update! Now you can effortlessly adjust Dicom tags via our public API, empowering seamless integration and customization. Experience improved PNG loading, including support for files with unexpected end of file (EOF), alongside optimized PNG loader performance. Convert DJVU files to PDF with ease, ensuring the first page is not blank. Plus, tackle EMF to PDF conversions effortlessly with text wrapping enhancements. We resolve issues with converting CDR images to DXF format. Enjoy smoother EPS to SVG exports with fixes for processing errors and missing text. Witness a significant performance boost in exporting large SVG files. Get ready for enhanced productivity with our latest PS (EPS) file export fixes. Upgrade now and streamline your workflow with precision and efficiency!
</p>

### New Feature - Edit DICOM Image Tags

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the most recent update, you now can modify DICOM image tags. You can achieve this by updating an existing tag using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.dicom/dicomimageinfo/updatetagat/">UpdateTagAt() method</a>, adding a new tag with <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.dicom/dicomimageinfo/addtag/">AddTag() methid</a>, or completely removing a tag using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.dicom/dicomimageinfo/removetagat/">RemoveTagAt() method</a>. Below is a C# code example demonstrating how to load a DICOM image, edit its tags, and then save the edited output images.
</p>

```cs
using (DicomImage image = (DicomImage)Image.Load("ttfm.dcm"))
{
    image.FileInfo.UpdateTagAt(33, "Test Patient"); // "Patient's Name"
    image.FileInfo.AddTag("Angular View Vector", 234);
    image.FileInfo.RemoveTagAt(29); // "Station Name"

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


## Aspose.Imaging for .NET 23.12

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Discover enhanced capabilities with our latest release. Introducing powerful additions to our API arsenal: `RemoveBackground` and `ChangeBackground` functionalities now support vector image processing, empowering seamless manipulation of visual elements. Experience smoother workflows as we resolve critical issues encountered during PNG export processes. Fixed `System.NullReferenceException` errors when exporting loaded PNGs with 64 bpp to 32 bpp, ensuring seamless transitions and flawless output. Moreover, streamline your operations with optimized `DataStreamSupporter.Save` functionalities, eliminating interruptions in your export procedures. Additionally, we've addressed conversion challenges, ensuring smooth transitions from EMF files to PDF formats. Fixed issues when you resize PNG images, enhancing your image management capabilities. Plus, enjoy uninterrupted functionality as EMF files seamlessly convert to SVG even in trial mode.
</p>

### New Feature - Remove and Change Background for Vector Images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging for .NET now offers robust background removal capabilities not only for raster images but also for vector formats like SVG, EMF, and CDR. Unlike raster images, background removal in vector files involves identifying and isolating objects without underlying shapes considered part of the background. The library allows you to specify a background color for removal, excluding foreground elements of the same color. Additionally, targeted background removal within specific areas of the image is possible. Removed backgrounds with the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/vectorimage/removebackground/">RemoveBackground() method</a> of `VectorImage` class, can be replaced with a new color or saved as foreground shapes on a transparent layer, providing flexibility and precision in image editing. To access C# code snippets and image examples illustrating background removal before and after, please refer to our Developer Guide article <a href="https://docs.aspose.com/imaging/net/removing-background-from-vector-images/">"Remove background from vector images in C#"</a>. It contains detailed demonstrations that will guide you through the process effectively.
</p>

Upgrade today and increase efficiency in your image processing workflows. You can find additional insights and explanations in the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-12-release-notes/">Aspose.Imaging 23.12 release notes</a>.

## Aspose.Imaging for .NET 23.11

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Experience enhanced versatility with our latest update. Seamlessly implement text styles such as italic and underline in CDR format, enriching your design possibilities with greater flexibility and precision. Streamline your workflows with improved PNG to PSD conversions, ensuring seamless transitions and preserving image integrity. We've resolved issues opening CMX files and converting them to PNG format. Additionally, EMF files are accurately converted to PNG, eliminating discrepancies and preserving visual quality. Fixed `System.NullReferenceException` errors encountered during specific CDR to PNG conversions, ensuring smooth and reliable operations. Furthermore, experience smoother SVG to PNG conversions as we address underlying issues, ensuring consistent and reliable outcomes.
</p>

### New Feature - Italic and Underline Text Styles in CDR Format

```cs
var baseFolder = "D:\\";
FontSettings.SetFontsFolder(Path.Combine(baseFolder, "Fonts"));
using (var image = Image.Load(Path.Combine(baseFolder, "Test.cdr")))
{
    image.Save(Path.Combine(baseFolder, "Test.cdr.jpg"));
}
```

## Aspose.Imaging for .NET 23.10
