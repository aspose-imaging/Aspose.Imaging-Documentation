---
type: docs
weight: '60'
url: /net/aspose-imaging-for-net-23-6-release-notes/
title: Aspose.Imaging for .NET 23.6 - Release notes
---

## Competitive features:
Switch to Aspose.Drawing as default graphics engine on Linux from libdgi

**Net2.0, Net3.5,Net3.5 client profile remove notice** - Please note, in the nearest releases Net2.0, Net3.5, Net3.5 client profile configurations will not be supported.

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGNET-6312 | Evaluation watermark is added to the output when converting DCM                                                                                                                                  | Enhancement      |
| IMAGINGNET-6283 | EMF to SVG NullReferenceException                                                                                                                                  | Enhancement      |
| IMAGINGNET-6110 | Regression: Exif Data is missing exception                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

Class    Aspose.Imaging.Masking.IMaskingAsyncTask

Field/Enum    Aspose.Imaging.FileFormats.Tiff.Enums.TiffExpectedFormat.TiffDeflateCmyk

Field/Enum    Aspose.Imaging.FileFormats.Tiff.Enums.TiffExpectedFormat.TiffDeflateCmyka

Field/Enum    Aspose.Imaging.FileFormats.Tiff.Enums.TiffExpectedFormat.TiffLzwCmyka

Field/Enum    Aspose.Imaging.FileFormats.Tiff.Enums.TiffExpectedFormat.TiffNoCompressionCmyk

Field/Enum    Aspose.Imaging.FileFormats.Tiff.Enums.TiffExpectedFormat.TiffNoCompressionCmyka

Method    Aspose.Imaging.CmykColorHelper.ToCmykaBytes(System.Int32[],System.Int32,System.Int32)

Method    Aspose.Imaging.CmykColorHelper.ToCmykaIccBytes
(System.Int32[],System.Int32,System.Int32,System.IO.Stream,System.IO.Stream)

Method    Aspose.Imaging.FileFormats.Tiff.FileManagement.TiffStreamWriter.Write
(System.IO.MemoryStream)

ethod    Aspose.Imaging.ImageOptions.IcoOptions.#ctor

Method    Aspose.Imaging.ImageOptions.TiffOptions.RemoveTags
(Aspose.Imaging.FileFormats.Tiff.Enums.TiffTags[])

Method    Aspose.Imaging.Masking.IMaskingAsyncTask.GetError

Method    Aspose.Imaging.Masking.IMaskingAsyncTask.GetMaskingResult



### Removed APIs:

## Usage Examples:

**IMAGINGNET-6312 Evaluation watermark is added to the output when converting DCM**

{{< highlight csharp >}}

using var stream = File.OpenRead(FileName);
using var image = ImagingVentureLicenser.Load(stream, true, string.Empty);
image.Save("output.png");

{{< /highlight >}}

**IMAGINGNET-6283 EMF to SVG NullReferenceException**

{{< highlight csharp >}}

cpp
using (EmfImage image = (EmfImage)Image.Load("D:\\SimpleReport.emf"))
{
   image.Save("D:\\result.svg", new SvgOptions());
}

{{< /highlight >}}

**IMAGINGNET-6110 Regression: Exif Data is missing exception**

{{< highlight csharp >}}

using var image = Image.Load(str, new LoadOptions { DataRecoveryMode = DataRecoveryMode.ConsistentRecover }) as JpegImage;

var exifData = image.ExifData;
if (exifData == null)
{
    throw new Exception("ExifData is missing");
}

// Do something with it
var bps = exifData.BitsPerSample;

{{< /highlight >}}

