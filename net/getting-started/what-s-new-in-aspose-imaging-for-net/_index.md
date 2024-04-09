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
Experience enhanced versatility with our latest update. Seamlessly implement text styles such as `italic` and `underline` in CDR format, enriching your design possibilities with greater flexibility. Streamline your workflows with improved PNG to PSD conversions, ensuring seamless transitions and preserving image integrity. We've resolved issues opening CMX files and converting them to PNG format. Additionally, EMF files are accurately converted to PNG, eliminating discrepancies and preserving visual quality. Fixed `System.NullReferenceException` errors encountered during specific CDR to PNG conversions, ensuring smooth and reliable operations. Furthermore, experience smoother SVG to PNG conversions as we address underlying issues, ensuring consistent and reliable outcomes.
</p>

### New Feature - Italic and Underline Text Styles in CDR Format

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Introducing enhanced font support for italic and underline styles in CDR file format! Seamlessly incorporate fonts with these styles into your designs by simply adding a font folder using the `FontSettings.SetFontsFolder()` method. Harness the power of this functionality with ease by following the C# example provided below:
</p>

```cs
var baseFolder = "D:\\";
FontSettings.SetFontsFolder(Path.Combine(baseFolder, "Fonts"));
using (var image = Image.Load(Path.Combine(baseFolder, "Test.cdr")))
{
    image.Save(Path.Combine(baseFolder, "Test.cdr.jpg"));
}
```

For additional information, please refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-11-release-notes/">Aspose.Imaging 23.11 release notes</a>.

## Aspose.Imaging for .NET 23.10

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the release of Aspose.Imaging 23.10, significant changes have been implemented to enhance the interface and behavior of the `EpsImage` class for EPS file manipulation. Here's a summary of the key points:

* **EpsType Enumeration**: Utilize the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.eps.consts/epstype/">EpsImage.EpsType property</a> to retrieve the file sub-type, as the `EpsInterchangeImage` and `EpsBinaryImage classes` have been deprecated.

* **Preview Image Retrieval**: To obtain a specific preview image or a list of all preview images, utilize the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.eps/epsimage/getpreviewimage/">EpsImage.GetPreviewImage(EpsPreviewFormat) method</a> or access the EpsImage.PreviewImages property. This replaces the usage of `EpsLoadOptions.PreviewExportFormat` and `EpsRasterizationOptions.PreviewToExport` properties, which have been removed.

* **EPS File Export**: Export EPS file renders using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/image/save/#imagesave-method-5-of-6">EpsImage.Save(Stream, ImageOptionsBase) method</a>. `The EpsPreviewFormat.PostScriptRendering` property is no longer available.

These changes streamline EPS file manipulation, providing a more intuitive and efficient workflow. Upgrade to Imaging 23.10 to leverage these enhancements and optimize your EPS file handling processes.
</p>

For further details, please consult the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-10-release-notes/">Aspose.Imaging 23.10 release notes</a>.

## Aspose.Imaging for .NET 23.9

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Introducing the latest advancements in Aspsoe.Imaging version 23.10, designed to streamline your image processing workflows while enhancing performance and reliability. Among the notable updates is the implementation of a <strong>Remove Watermark filter</strong>, empowering users to effortlessly eliminate unwanted overlays and refine images. Additionally, we've addressed issues such as the "Required palette is missing" exception encountered during BMP loading, ensuring uninterrupted workflows. Furthermore, enhancements have been made to address GIF file loading issues, providing a smoother user experience. Our team has also resolved exceptions occurring during palette creation for large images, ensuring stability in image processing tasks. Moreover, improvements have been made to DICOM file loading to ensure accurate rendering and reliable data retrieval. Lastly, we've resolved errors encountered when inheriting custom classes from Image, ensuring seamless integration and compatibility.
</p>

<em>Please note: With this release, we've made changes regarding the .NET 5 configuration. Aspose.Imaging version 23.10 will no longer support .NET 5 configurations.</em>

### New Feature - Remove watermark filter

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A new feature called the Remove Watermark Image Filter managed through the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark/watermarkremover/">WatermarkRemover class</a>, enables users to remove unwanted watermarks, such as manufacturer logos or device model names, from photos captured by certain smartphones and cameras. This filter provides a convenient solution for users who need to share photos without these unwanted marks, enhancing the overall quality and presentation of their images.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Here's a simple example of how you can use the `WatermarkRemover` class in C# for watermark removal:
</p>

```cs
var imageFilePath = "ball.png";
var outputFilePath = "result.png";
using (var image = Image.Load(imageFilePath))
{
    var pngImage = (PngImage)image;

    var mask = new GraphicsPath();
    var firstFigure = new Figure();
    firstFigure.AddShape(new EllipseShape(new RectangleF(350, 170, 570 - 350, 400 - 170)));
    mask.AddFigure(firstFigure);

    var options = new ContentAwareFillWatermarkOptions(mask)
    {
        MaxPaintingAttempts = 4
    };

    var result = WatermarkRemover.PaintOver(pngImage, options);

    result .Save(outputFilePath);
}
```
<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a more detailed explanation with pictures and further information, please refer to our Developer Guide article <a href="https://docs.aspose.com/imaging/net/developer-guide/manipulating-images/image-and-photo-filters/#remove-watermark-image-filter">"Remove Watermark Image Filter"</a>.
</p>

For more in-depth information, please refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-9-release-notes/">Aspose.Imaging 23.9 release notes</a> for additional details and updates.

## Aspose.Imaging for .NET 23.8

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Our latest update introduced the implementation of the <strong>Magic Wand tool</strong>, offering precise selection capabilities to refine your designs with ease. Furthermore, we've diligently addressed bugs related to font rendering during SVG exports, ensuring that your text elements retain their intended appearance without compromise. In addition, our team has resolved issues pertaining to the saving of images with dimensions exceeding 65535 pixels to JPEG format, guaranteeing accurate and reliable output for your high-resolution projects. Moreover, we've implemented improvements for exporting multi-frame GIFs to composite image formats, providing a seamless and efficient workflow for handling animated content.
</p>

### New Feature - Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Magic Wand tool is indispensable for graphic designers, allowing easy selection of specific color areas in images or photos. By utilizing the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.magicwand/magicwandtool/">MagicWandTool class</a> from the Aspose.Imaging library, designers can select a color area by simply choosing a point within it. The tool automatically extends the selection to include all adjacent areas sharing a similar color, streamlining complex selections and adjustments.
</p>

C# code example:
```cs
using (RasterImage image = (RasterImage)Image.Load("src.png"))
{
    // Create a new mask using magic wand tool based on tone and color of pixel {845, 128}
    MagicWandTool.Select(image, new MagicWandSettings(845, 128))
        // Union the existing mask with the specified one created by magic wand tool
        .Union(new MagicWandSettings(416, 387))
        // Invert the existing mask
        .Invert()
        // Subtract the specified mask created by magic wand tool from the existing one
        .Subtract(new MagicWandSettings(1482, 346) { Threshold = 69 })
        // Subtract four specified rectangle masks from the existing mask one by one
        .Subtract(new RectangleMask(0, 0, 800, 150))
        .Subtract(new RectangleMask(0, 380, 600, 220))
        .Subtract(new RectangleMask(930, 520, 110, 40))
        .Subtract(new RectangleMask(1370, 400, 120, 200))
        // Feather mask with specified settings
        .GetFeathered(new FeatheringSettings() { Size = 3 })
        // Apply mask to the image
        .Apply();
    image.Save("output.png");
}
```
<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a comprehensive explanation accompanied by images and additional information, please consult our Developer Guide article <a href="https://docs.aspose.com/imaging/net/developer-guide/manipulating-images/image-and-photo-filters/#magic-wand-tool">"Magic Wand tool"</a>.
</p>

If you require more detailed information, we recommend you refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-8-release-notes/">Aspose.Imaging 23.8 release notes</a>.

## Aspose.Imaging for .NET 23.7

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the addition of the alpha blending feature for `RasterImage`, you now have even greater control over transparency and layering in your projects, allowing for more dynamic compositions and effects. Additionally, we've resolved issues related to EMF export errors, ensuring seamless compatibility. Furthermore, our team has diligently addressed concerns regarding the CCITT G3 1D decoder, ensuring that it functions properly and delivers reliable results. Moreover, we've made improvements to the synchronization of page management and format-specific collections for multi-page images, enhancing the consistency and efficiency of your image processing tasks.
</p>

<em>Please note: In line with our commitment to advancing technology, we have discontinued support for configurations utilizing .NET 2.0, .NET 3.5, and .NET 3.5 client profile since Aspose.Imaging version 23.7.</em>

### New Feature - Alpha Blending

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In today's online landscape, captivating users is increasingly challenging. However, beyond artistic endeavors, <strong>Alpha Blending</strong> image filters play a crucial role, particularly in watermarking images. They not only assert ownership but also promote individual or corporate identity effectively. By overlaying a semi-transparent logo onto the original document, the author's ownership is established discreetly yet prominently. The provided C# code example demonstrates the application of this technique, utilizing the  <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/blend/">Blend() method</a> from the `RasterImage` class. This method seamlessly combines two images, background and overlay, enabling the efficient creation of visually engaging compositions, including watermarks, with ease.
</p>

```cs
using var background = Image.Load("background.webp") as RasterImage;
using var overlay = Image.Load("logo.png") as RasterImage;

var center = new Point((background.Width - overlay.Width) / 2, (background.Height - overlay.Height) / 2);
background.Blend(center, overlay, overlay.Bounds, 127);

background.Save("blended.webp");
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Please explore our Developers Guide article <a href="https://docs.aspose.com/imaging/net/developer-guide/manipulating-images/image-and-photo-filters/#alpha-blending-image-filter">"Alpha Blending Image Filter"</a> for more detailed explanations accompanied by image examples.
</p>

For more information about the release, please visit the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-7-release-notes/">Aspose.Imaging 23.7 release notes</a>.

## Aspose.Imaging for .NET 23.6

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With our latest update, we've addressed several key issues to provide you with a smoother and more reliable workflow. Firstly, we've resolved the occurrence of evaluation watermarks being inadvertently added to output files when converting DCM images. Furthermore, we've tackled a `NullReferenceException` error that occurred when converting EMF files to SVG format. This fix ensures that your conversions proceed smoothly and without interruption. Additionally, we've addressed a regression issue where EXIF data was missing, leading to exceptions during image processing. With this fix in place, you can rest assured that your images will retain their metadata intact, allowing for more accurate organization and management.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the release of version 23.6, Aspose.Imaging for .NET now fully supports <a href="https://products.aspose.com/drawing/net/">Aspose.Drawing</a> for .NET7 configuration as the default graphics engine. This integration brings a host of benefits, including advanced rendering capabilities, improved efficiency and compatibility.
</p>

For further details about the release, please visit the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-6-release-notes/">Aspose.Imaging 23.6 release notes</a>.

## Aspose.Imaging for .NET 23.5

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
We're pleased to unveil our latest Imaging graphic library update, introducing a range of enhancements tailored to optimize your image processing workflows. Among the notable additions are support for tiled TIFF writing, rectifying the incorrect orientation issue with WMF rendering, and ensuring accurate arrow rendering when converting SVG files to PDF format. Additionally, we now support TIFF files with CMYK Alpha color mode, as well as seamless conversion of PNG images to TIFF while preserving CMYK colorspace and transparency. Furthermore, we've addressed exceptions encountered during PNG file rendering to PNG format. Experience enhanced efficiency and precision in your image processing tasks with our latest release.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
We've introduced support for .NET7 configuration, providing you with even greater flexibility and compatibility in your development environment. Now, you can seamlessly integrate our Imaging library into your .NET7 projects.
</p>

### New Feature - TIFF Tiled Writing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The tiled TIFF writing feature empowers you to efficiently handle large images with ease. Below is a sample C# code demonstrating how to load and save tiled TIFF files:
</p>

```cs
using var image = Image.Load("tiled-tiff.tiff") as TiffImage;

var page = image.Pages[0] as TiffFrame;
if (page.FrameOptions.IsTiled)
{
    Console.WriteLine("Tiff is tiled");
}

image.Save("output-tiled.tiff");
```

For additional details about the release, please refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-5-release-notes/">Aspose.Imaging 23.5 release notes</a>.

## Aspose.Imaging for .NET 23.4

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Introducing our latest release, packed with enhancements to elevate your image processing workflows. Key highlights include support for rendering image raw data from EPS files, providing greater flexibility and control over your designs. Additionally, we've removed the usage of unsafe `BinaryFormatter`, ensuring improved security and reliability in serialization tasks. Addressing compatibility concerns, we've resolved DICOM loading issues under ARM64 mode, ensuring seamless operations across different platforms. Furthermore, we've rectified export inconsistencies, such as bottom-right shifted content in EMF images exported to PNG format and incorrect text offsets in EMF formulas rasterization. Plus, we've addressed issues related to object disposal after ICO image conversion, ensuring smoother transitions throughout your workflow. Upgrade now to experience these enhancements and optimize your image processing endeavors.
</p>

### New Feature - Image Raw Data Rendering from EPS

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The rendering of image raw data from EPS files provides enhanced flexibility and control over your image rendering process. Below is a code example in C# of exporting EPS files to PNG format:
</p>

```cs
var options = new EpsLoadOptions { PreviewExportFormat = EpsPreviewFormat.PostScriptRendering, };
using (var image = Image.Load("input.eps", options))
{
    image.Save("output.png");
}
```

For further information, please consult the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-4-release-notes/">Aspose.Imaging 23.4 release notes</a>.

## Aspose.Imaging for .NET 23.3

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Announcing our latest release, featuring a range of enhancements to elevate your image processing experience. With added support for BigTIFF, handling larger image files is now more seamless than ever. Also, we've fixed compatibility issues when resultant PNG files opened in Photoshop. Additionally, we've addressed a specific issue on Linux systems where attempting to convert EMZ files resulted in a "Cannot access a closed file" error. Furthermore, improvements have been made to the functionality of `WmfImage.Crop`, resolving inaccuracies and preventing exceptions with certain files. Upgrade now to access these enhancements and optimize your image processing workflows.
</p>

### New Feature - BigTIFF Image Support

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.fileformats.bigtiff/bigtiffimage/">BigTiffImage class</a> implementation, you can now effortlessly handle larger image files with ease. Here's an example of loading and exporting BigTIFF images in C#:
</p>

```cs
var inputPath = "input-BigTIFF.tif";
var outputPath = "output-BigTIFF.tif";

using (var image = Image.Load(inputPath) as BigTiffImage)
{
    image.Save(outputPath, new BigTiffOptions(TiffExpectedFormat.TiffLzwRgba));
}
```

For more detailed information, please check the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-3-release-notes/">Aspose.Imaging 23.3 release notes</a>.

## Aspose.Imaging for .NET 23.2


### New Feature - Plugin Licensing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging now introduces Plugin licensing, enabling access to specific features and functions tailored to your needs. With support for .NET Standard 2.0 and higher configurations, you can now acquire licenses for the exact capabilities you require. Our Plugin licensing system ensures you get precisely what you need, maximizing efficiency and minimizing unnecessary costs.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To acquire Plugin licenses or learn more about available options, please visit our <a href="https://purchase.aspose.org/imaging">Purchase page</a>. Additionally, detailed descriptions of available plugins can be found in the <a href="/imaging/net/aspose-imaging-net-licensing-plugins/">Licensing Plugins Documentation</a>. This provides you with comprehensive information to make informed decisions about which plugins best suit your requirements.
</p>

Example of using Licensing plugin in C#:
```cs
// Valid plugin license use example
Metered license = new Metered();
// Only one metered plug-in license is supported
license.SetMeteredKey("<your public key>", "<your private key>");
```

### New Feature - Export Indexed PNG Images with Transparency

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The latest release introduced the ability to maintain transparency when indexing PNG images. Here's a C# code example illustrating how to load a PNG image with an alpha channel and save it with indexed colors while preserving transparency:
</p>

```cs
using (RasterImage image = (RasterImage)Image.Load("input_png_with_alpha.png"))
{
    PngOptions options = new PngOptions()
    {
        CompressionLevel = 9,
        ColorType = PngColorType.IndexedColor,
        Palette = ColorPaletteHelper.GetCloseTransparentImagePalette(image, 256),
        FilterType = PngFilterType.Avg,
    };

    image.Save("input_png_with_alpha.png.png", options);
}
```

For further insights, please review the <a href="https://releases.aspose.com/imaging/net/release-notes/2023/aspose-imaging-for-net-23-2-release-notes/">Aspose.Imaging 23.2 release notes</a>.
