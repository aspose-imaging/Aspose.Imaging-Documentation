---
type: docs
weight: '60'
url: /net/aspose-imaging-for-net-20-12-release-notes/
title: Aspose.Imaging for .NET 20.12 - Release notes
---

**Competitive features:**
-----------------------

**Changes:**

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGNET-4215 | Implement public API to determine if the palette is used by the image                                                                                                                                  | Feature      |
| IMAGINGNET-4154 | Implement the ability to create animation from an array of images                                                                                                                                  | Feature      |
| IMAGINGNET-4144 | Support for access to missing Exif properties                                                                                                                                  | Feature      |
| IMAGINGNET-4233 | Tga Creator always creates corrupted images                                                                                                                                  | Enhancement      |
| IMAGINGNET-4227 | Improve GraphCutHelper performance and async implementation                                                                                                                                  | Enhancement      |
| IMAGINGNET-4194 | Exception during the export from EMF to PNG file format                                                                                                                                  | Enhancement      |
| IMAGINGNET-4190 | Image export failed exception when converting BMP to PNG                                                                                                                                  | Enhancement      |
| IMAGINGNET-4187 | Resize, Crop, RotateFlip and Rotate methods of TgaImage don't work                                                                                                                                  | Enhancement      |
| IMAGINGNET-4155 | Exception on combining Tiff                                                                                                                                  | Enhancement      |
| IMAGINGNET-4010 | Rework multipage image related methods and properties to be user-friendly                                                                                                                                  | Enhancement      |

**Public API changes:**
-----------------------

**Added APIs:**

Class    Aspose.Imaging.Exif.MakerNote

Class    Aspose.Imaging.ImageOptions.TimeInterval

Class    Aspose.Imaging.Masking.Result.IMaskingLayer

Field/Enum    Aspose.Imaging.ImageOptions.MultiPageMode.TimeInterval

Field/Enum    Aspose.Imaging.Masking.Result.MaskingResult.MaskingArea

Field/Enum    Aspose.Imaging.Masking.Result.MaskingResult.OriginImage

Method    Aspose.Imaging.AsyncTask.IAsyncTaskState.IncrementProgressMaxValue(System.Int32)

Method    Aspose.Imaging.AsyncTask.IAsyncTaskState.IndicateProgress(Aspose.Imaging.ProgressManagement.EventType)

Method    Aspose.Imaging.Exif.MakerNote.ToString

Method    Aspose.Imaging.FileFormats.Tga.TgaImage.Crop(Aspose.Imaging.Rectangle)

Method    Aspose.Imaging.FileFormats.Tga.TgaImage.Crop(System.Int32,System.Int32,System.Int32,System.Int32)

Method    Aspose.Imaging.FileFormats.Tga.TgaImage.Resize(System.Int32,System.Int32,Aspose.Imaging.ImageResizeSettings)

Method    Aspose.Imaging.FileFormats.Tga.TgaImage.Resize(System.Int32,System.Int32,Aspose.Imaging.ResizeType)

Method    Aspose.Imaging.FileFormats.Tga.TgaImage.Rotate(System.Single,System.Boolean,Aspose.Imaging.Color)

Method    Aspose.Imaging.FileFormats.Tiff.TiffTagTypes.TiffUndefinedType.CopyInstanceData(Aspose.Imaging.FileFormats.Tiff.TiffDataType)

Method    Aspose.Imaging.FileFormats.Tiff.TiffTagTypes.TiffUndefinedType.CreateInstance

Method    Aspose.Imaging.FileFormats.Tiff.TiffTagTypes.TiffUndefinedType.ReadData(Aspose.Imaging.FileFormats.Tiff.FileManagement.TiffStreamReader,System.Int64,System.Int64)

Method    Aspose.Imaging.FileFormats.Tiff.TiffTagTypes.TiffUndefinedType.WriteTagValueOrOffset(Aspose.Imaging.FileFormats.Tiff.FileManagement.TiffStreamWriter,System.Int64)

Method    Aspose.Imaging.Image.Create(Aspose.Imaging.Image[])

Method    Aspose.Imaging.Image.Create(Aspose.Imaging.Image[],System.Boolean)

Method    Aspose.Imaging.ImageOptions.TimeInterval.#ctor(System.UInt32,System.UInt32)

Method    Aspose.Imaging.Masking.ImageMasking.ApplyMask(Aspose.Imaging.RasterImage,Aspose.Imaging.RasterImage,Aspose.Imaging.Masking.Options.MaskingOptions)

Method    Aspose.Imaging.Masking.ImageMasking.LoadSession(System.IO.Stream)

Method    Aspose.Imaging.Masking.ImageMasking.LoadSession(System.String)

Method    Aspose.Imaging.Masking.IMaskingSession.Save(System.IO.Stream)

Method    Aspose.Imaging.Masking.IMaskingSession.Save(System.String)

Method    Aspose.Imaging.Masking.Result.IMaskingLayer.GetImage

Method    Aspose.Imaging.Masking.Result.IMaskingLayer.GetMask

Method    Aspose.Imaging.Masking.Result.MaskingResult.#ctor(Aspose.Imaging.Masking.Options.MaskingOptions,Aspose.Imaging.RasterImage,Aspose.Imaging.Rectangle)

Method    Aspose.Imaging.Masking.Result.MaskingResult.GetEnumerator

Property    Aspose.Imaging.AsyncTask.IAsyncTask.ProgressEventHandler

Property    Aspose.Imaging.Exif.ExifData.Make

Property    Aspose.Imaging.Exif.ExifData.MakerNotes

Property    Aspose.Imaging.Exif.MakerNote.Name

Property    Aspose.Imaging.Exif.MakerNote.Value

Property    Aspose.Imaging.FileFormats.Tga.TgaImage.FileFormat

Property    Aspose.Imaging.Image.UsePalette

Property    Aspose.Imaging.ImageLoadOptions.Jpeg2000LoadOptions.MaximumDecodingTimeForTile

Property    Aspose.Imaging.ImageOptions.MultiPageOptions.TimeInterval

Property    Aspose.Imaging.ImageOptions.TimeInterval.From

Property    Aspose.Imaging.ImageOptions.TimeInterval.To

Property    Aspose.Imaging.Masking.Options.AutoMaskingGraphCutOptions.PrecalculationProgressEventHandler

Property    Aspose.Imaging.Masking.Result.IMaskingLayer.ObjectNumber

Property    Aspose.Imaging.Masking.Result.MaskingResult.Item(System.Int32)

Property    Aspose.Imaging.Masking.Result.MaskingResult.Layers

Property    Aspose.Imaging.Masking.Result.MaskingResult.Length

Property    Aspose.Imaging.RasterImage.UsePalette



**Removed APIs:**

Class    Aspose.Imaging.AsyncTask.ProgressCallback

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Backpack

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Bottle

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Bowl

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Dog

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Orange

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.SportsBall

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Tie

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.TV

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Umbrella

Field/Enum    Aspose.Imaging.Masking.Options.DetectedObjectType.Vase

Method    Aspose.Imaging.AsyncTask.IAsyncTask.SetProgressCallback(Aspose.Imaging.AsyncTask.ProgressCallback)

Method    Aspose.Imaging.AsyncTask.IAsyncTaskState.SetProgress(System.Int32)

Method    Aspose.Imaging.FileFormats.Gif.GifImage.RotateFlipAll(Aspose.Imaging.RotateFlipType)

Method    Aspose.Imaging.Masking.Result.MaskingResult.#ctor(Aspose.Imaging.Masking.Options.MaskingOptions,System.Int32)

Method    Aspose.Imaging.Masking.Result.MaskingResult.GetImage

Property    Aspose.Imaging.AsyncTask.IAsyncTask.Progress

Property    Aspose.Imaging.Exif.JpegExifData.Make

Property    Aspose.Imaging.Masking.Result.MaskingResult.ObjectNumber

**Usage Examples:**
-----------------------

**IMAGINGNET-4233 Tga Creator always creates corrupted images**

```
### Creating new Tga image with a centered red circle 

var options = new TgaOptions
                  {
                      Source = new FileCreateSource("output.tga", false)
                  };

using (var image = Image.Create(options, 1000, 1000))
{
    var graphics = new Graphics(image);
    graphics.FillEllipse(new SolidBrush(Color.Red), 300, 300, 400, 400);
    image.Save();
}
```

**IMAGINGNET-4215 Implement public API to determine if the palette is used by the image**

```
using (var image = Image.Load(folder + "Sample.bmp"))
{
     if (image.UsePalette)
     {
          Console.WriteLine("The palette is used by the image");
     }
}
```

**IMAGINGNET-4194 Exception during the export from EMF to PNG file format**

```
using (var image = Image.Load("LetterHeadWW.emf"))
{
    image.Save("result.png", new PngOptions());
}
```

**IMAGINGNET-4190 Image export failed exception when converting BMP to PNG**

```
### Receiving a detailed error message loading corrupted image



try
{
    using (var image = Image.Load("design.bmp"))
    {
        PngOptions pngOptions = new PngOptions();
        image.Save("output.png", pngOptions);
    }
}
catch (ImageSaveException e)
{
    bool hasExpectedExceptionMessage = e.InnerException.InnerException.Message == "Required palette is missing. Image data loading failed.";
    if (!hasExpectedExceptionMessage)
    {
        throw;
    }
}
```

**IMAGINGNET-4187 Resize, Crop, RotateFlip and Rotate methods of TgaImage don't work**

```
### Cropping a TGA image


            using (RasterImage sampleTgaImage = (RasterImage)Image.Load("test.tga"))
            {
                sampleTgaImage.Crop(10, 10, 10, 10);
                sampleTgaImage.Save("crop.tga");
            }


### Rotating a TGA image


            using (RasterImage sampleTgaImage = (RasterImage)Image.Load("test.tga"))
            {
                sampleTgaImage.Rotate(30);
                sampleTgaImage.Save("rotate.tga");
            }


### Resizing a TGA image


            using (RasterImage sampleTgaImage = (RasterImage)Image.Load("test.tga"))
            {
                sampleTgaImage.Resize(100, 100);
                sampleTgaImage.Save("resize.tga");
            }


### Flip-rotating a TGA image


            using (RasterImage sampleTgaImage = (RasterImage)Image.Load("test.tga"))
            {
                sampleTgaImage.RotateFlip(RotateFlipType.Rotate270FlipXY);
                sampleTgaImage.Save("rotate_flip.tga");
            }
```

**IMAGINGNET-4155 Exception on combining Tiff**

```
using (var page1 = (TiffImage)Image.Load("Image1.tif"))
{
    using (var page2 = (TiffImage)Image.Load("Image2.tif"))
    {
        page1.AddFrame(TiffFrame.CopyFrame(page2.ActiveFrame));
    }

    page1.Save("Result.tif");
}
```

**IMAGINGNET-4154 Implement the ability to create animation from an array of images**

```
input files in test.zip


string baseFolder = Path.Combine(@"D:\", "test");
string outFileName = "MultipageImageCreateTest.tif";
string outputFilePath = Path.Combine(baseFolder, outFileName);
string[] files = new string[]{ "33266.tif", "Animation.gif", "elephant.png", "Input.jp2", 
"eye.wmf", "tiger.bmp", "MultiPage.cdr", "juanmontoya_lingerie.svg" };
List<Image> images = new List<Image>();
foreach (var file in files)
{
   string filePath = Path.Combine(baseFolder, file);
   images.Add(Image.Load(filePath));
}

using (Image image = Image.Create(images.ToArray(), true))
{
   image.Save(outputFilePath, new TiffOptions(TiffExpectedFormat.TiffJpegRgb));
}
```

**IMAGINGNET-4144 Support for access to missing Exif properties**

```
using (var image = (JpegImage)Image.Load("Sample.jpg"))
{
    foreach (var makerNote in image.ExifData.MakerNotes)
    {
        Console.WriteLine("{0}: {1}", makerNote.Name, makerNote.Value);
    }

    Console.ReadKey();
}
```

**IMAGINGNET-4010 Rework multipage image related methods and properties to be user-friendly**

```
string baseFolder = Path.Combine(@"D:\", "test");
string outFileName = "MultipageImageCreateTest.tif";
string outputFilePath = Path.Combine(baseFolder, outFileName);
string[] files = new string[]{ "33266.tif", "Animation.gif", "elephant.png", "Input.jp2", 
"eye.wmf", "tiger.bmp", "MultiPage.cdr", "juanmontoya_lingerie.svg" };
List<Image> images = new List<Image>();
foreach (var file in files)
{
   string filePath = Path.Combine(baseFolder, file);
   images.Add(Image.Load(filePath));
}

using (Image image = Image.Create(images.ToArray(), true))
{
   image.Save(outputFilePath, new TiffOptions(TiffExpectedFormat.TiffJpegRgb));
}
```

