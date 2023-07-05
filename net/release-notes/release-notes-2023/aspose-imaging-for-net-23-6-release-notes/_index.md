---
type: docs
weight: '60'
url: /net/aspose-imaging-for-net-23-6-release-notes/
title: Aspose.Imaging for .NET 23.6 - Release notes
---

## Competitive features:
Since [23.6 release](https://www.nuget.org/packages/Aspose.Imaging/23.6.0) Aspose.Imaging for .NET supports [Aspose.Drawing](https://products.aspose.com/drawing/net/) for .NET7 configuration as default graphics engine. If you work with Aspose.Imaging in Non-Windows environment you can view [how to work with Aspose.Imaging .NET Core dlls in Non-Windows Environment](/imaging/net/installation/working-with-aspose-imaging-in-non-windows-environment/) guide.

**Net2.0, Net3.5,Net3.5 client profile remove notice** - Please note, in the nearest releases Net2.0, Net3.5, Net3.5 client profile configurations will not be supported.

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGNET-6312 | Evaluation watermark is added to the output when converting DCM                                                                                                                                  | Enhancement      |
| IMAGINGNET-6283 | EMF to SVG NullReferenceException                                                                                                                                  | Enhancement      |
| IMAGINGNET-6110 | Regression: Exif Data is missing exception                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

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

