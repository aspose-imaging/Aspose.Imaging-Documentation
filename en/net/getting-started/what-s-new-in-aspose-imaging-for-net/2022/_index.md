---
title: News Archive 2022
type: docs
weight: 10
url: /net/what-s-new-in-aspose-imaging-for-net/2022/
keywords: C# image library, C# image processing, image processing features, imaging API enhancements, Imaging recent releases, graphic processing, image manipulation, raster file formats, conversion options, create method, speed up creation, 64 bit PNG images
description: Aspose.Imaging new features and enhancements introduced in our recent releases, empowering you to unlock new possibilities in graphic processing and manipulation. Support for the most common raster file formats, alongside a diverse array of conversion options.
---

{{% alert color="primary" %}}

This page highlights the new features and enhancements introduced in recent releases of Aspose.Imaging graphic library. Your feedback is invaluable to us as we strive to improve our product. We greatly appreciate it if you take a moment to provide your insights on different aspects and complete the <a href="https://forms.gle/LRjHCzSrjfiqrkPQ6">Aspose.Imaging for .NET feedback form</a>.

{{% /alert %}}

<a href="/imaging/net/what-s-new-in-aspose-imaging-for-net/">< What's New in Aspose.Imaging for .NET</a>

## Aspose.Imaging for .NET 22.12

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the latest update of Aspose.Imaging, we've introduced several exciting new features and enhancements:

- Enhance speed in **creating methods** within the Aspose.Imaging graphic library for improved efficiency.
- Address distortion in output images when **converting SVG to PNG** format.
- Fix memory leak issue when **saving TIFF frames** to MemoryStream, ensuring optimal resource management.
- Resolve dynamic loading failure for **conversion to DICOM** format, ensuring seamless operations.
- Correct conversion discrepancies **from SVG to PNG format** for accurate rendering.
- Ensure accurate conversion of specific **TIFF images to PDF** format.
- Resolve loading issues with **CDR images** for uninterrupted access.
- Fix conversion errors for specific **CDR images to PDF** format for reliable output.
- Address **WebP export** failure to ensure successful exportation.
- Fix partial **PDF processing** issues during export for complete and accurate results.
</p>

### New Feature - Speed up create method

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The latest update focuses on enhancing the efficiency of the create method, leading to a notable boost in productivity. Users can now experience accelerated performance when initiating this code in the current version compared to the previous version. By conducting a comparative analysis between the two versions, users can observe tangible improvements in speed and productivity.
</p>

```cs
var imageSize = new Size(1000, 1000);
var colors = CreateColors();
var options = new BmpOptions();
Stopwatch s = new Stopwatch();
s.Start();
for (var i = 0; i < 500; i++)
{
    using (var ms = new MemoryStream())
    {
        options.Source = new StreamSource(ms);
        using (var image = (RasterImage) Image.Create(options, imageSize.Width, imageSize.Height))
        {
            image.SaveArgb32Pixels(image.Bounds, colors);
            image.Save();
        }
    }
}

s.Stop();
Console.WriteLine("{0:0.0000}sec", s.Elapsed.TotalSeconds);

private int[] CreateColors()
{
    var inputFile = @"D:\tiger.bmp";
    using (RasterImage image = (RasterImage)Image.Load(inputFile))
    {
        var colors = image.LoadArgb32Pixels(image.Bounds);
        return colors;
    }
}
```

For a deeper understanding, please refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2022/aspose-imaging-for-net-22-12-release-notes/">Aspose.Imaging 22.12 release notes</a>.

## Aspose.Imaging for .NET 22.11

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Boost your productivity with the latest enhancements in our release:

- Integrate **Aspose.Fonts into Aspose.Imaging** for enhanced functionality and versatility.
- Resolve issues with **converting DICOM images to APNG** format for seamless compatibility.
- Address loading errors with **WEBP images** to ensure proper access.
- Fix conversion errors when **converting CDR files to JPG** format for accurate output.
- Enhance **EMF formulas rasterization** for improved rendering and precision.
- Resolve conversion failures when **converting EMF files to SVG** format for reliable results.
- Ensure proper **conversion of EMF files to PNG** format for accurate representation.
</p>

### New Feature - Integration of Aspose.Fonts into Aspose.Imaging

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The integration of Aspose.Fonts into Aspose.Imaging allows for direct access to character indices, bypassing the Unicode table. This example showcases the capability of accessing character indices directly, which is supported by the EMF format. In the provided line of code, `text.WEmrText.Options = EmfExtTextOutOptions.ETO_GLYPH_INDEX;`, characters are accessed via GlyphIndex. It's important to note that the specified font must match the one used in the example, as the GlyphIndex for each font corresponds to different characters.
</p>

```cs
 const string baseFolder = "D:\\Test";
 const string fontName = "Cambria Math";
 const int symbolCount = 40; //count sybols in the example
 const int startIndex = 2001; //start GlyphIndex for example
 string fontFolder = Path.Combine(baseFolder, "Fonts"); //font folder
 FontSettings.SetFontsFolder(fontFolder);

 //Fill GlyphIndex buffer
 var glyphCodes = new int[symbolCount];
 for (int i = 0; i < symbolCount; i++)
 {
     glyphCodes[i] = startIndex + i;
 }

 //create emf
 using (EmfImage emf = new EmfImage(700,100))
 {
     //font record
     var font = new EmfExtCreateFontIndirectW();
     font.Elw = new EmfLogFont();
     font.Elw.Facename = fontName;
     font.Elw.Height = 30;

     //text record
     var text = new EmfExtTextOutW();
     text.WEmrText = new EmfText();
     text.WEmrText.Options = EmfExtTextOutOptions.ETO_GLYPH_INDEX; //symbols index as GlyphIndex
     text.WEmrText.Chars = symbolCount; //string length
     text.WEmrText.GlyphIndexBuffer = glyphCodes; //index buffer

     emf.Records.Add(font); //add font
     emf.Records.Add(new EmfSelectObject()
     {
         ObjectHandle = 0
     }); //select font
     emf.Records.Add(text); //add text
     emf.Save(Path.Combine(baseFolder,"result.png")); //rendering
 }
 ```

For additional information, please refer to the <a href="https://releases.aspose.com/imaging/net/release-notes/2022/aspose-imaging-for-net-22-11-release-notes/">Aspose.Imaging 22.11 release notes</a>.

## Aspose.Imaging for .NET 22.10

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Explore advanced features with our latest release:

- Introduce support for **16-bit/channel 64-bit PNG images** for enhanced color depth.
- Address exceptions encountered during **conversion of GIF and DICOM** images to BMP format for seamless operations.
- Resolve exceptions while loading particular **TIFF files** to ensure uninterrupted access.
- Address export failure for specific **SVG images** to guarantee successful exportation.
- Fix "Unknown character" exception when **opening ODG files** for improved compatibility.
- Correct color changes during **DNG to JPG conversion** to maintain image integrity.
- Ensure **PSD exporter** saves **CMYK colors as RGB** for accurate color representation.
</p>

<em>Please note: A new version has been added to support an alternative graphics engine, Aspose.Drawing, instead of System.Drawing.Common/GDI+, for configurations using .NET Standard 2.0 and higher. This enhancement provides users with more options and flexibility in choosing their preferred graphics engine.</em>

### New Feature - Support of 16-bit/Channel 64 bit PNG images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Support has been added for 16-bit/channel 64-bit PNG images. This means that PNG images with 16 bits per channel are now also compatible. Below is an example demonstrating how to load and save a 64-bit PNG image:
</p>

```cs
using (RasterImage image = (RasterImage)Image.Load("image0.png"))
{
    ImageOptionsBase options = image.GetOriginalOptions();
    image.Save("result.png", options);
}
```

Further insights and explanations are available in the <a href="https://releases.aspose.com/imaging/net/release-notes/2022/aspose-imaging-for-net-22-10-release-notes/">Aspose.Imaging 22.10 release notes</a>.
