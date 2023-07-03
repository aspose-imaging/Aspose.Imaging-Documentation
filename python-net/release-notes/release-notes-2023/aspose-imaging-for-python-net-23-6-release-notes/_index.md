---
type: docs
weight: '60'
url: /net/aspose-imaging-for-python-net-23-6-release-notes/
title: Aspose.Imaging for Python via .NET 23.6 - Release notes
---

## Competitive features:
Switch to Aspose.Drawing as default graphics engine on Linux from libdgi

| **Key**             | **Summary**                                                                                                                                                    |   **Category**   |
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|
| IMAGINGPYTHONNET-73 | EMF to SVG NullReferenceException                                                                                                                              | Enhancement      |
| IMAGINGPYTHONNET-74 | Regression: Exif Data is missing exception                                                                                                                     | Enhancement      |

## Public API changes:

### Added APIs:

Class    `aspose.imaging.masking.IMaskingAsyncTask`

Field/Enum    `aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat.TiffDeflateCmyk`

Field/Enum    `aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat.TiffDeflateCmyka`

Field/Enum    `aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat.TiffLzwCmyka`

Field/Enum    `aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat.TiffNoCompressionCmyk`

Field/Enum    `aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat.TiffNoCompressionCmyka`

Method    `aspose.imaging.CmykColorHelper.to_cmyka_bytes(argb_pixels, start_index, length)`

Method    `aspose.imaging.CmykColorHelper.to_cmyka_icc_bytes(pixels, start_index, length, rgb_icc_stream, cmyk_icc_stream)`

Constructor    `aspose.imaging.imageoptions.IcoOptions.__init(self)___`

Method    `aspose.imaging.imageoptions.TiffOptions.remove_tags(tags)`

Method    `aspose.imaging.masking.IMaskingAsyncTask.get_error`

Method    `aspose.imaging.masking.IMaskingAsyncTask.get_masking_result`


### Removed APIs:

## Usage Examples:

**IMAGINGPYTHONNET-73 EMF to SVG NullReferenceException**

{{< highlight python >}}

with Image.load("SimpleReport.emf") as image:
    image.save("result.svg", SvgOptions())

{{< /highlight >}}

**IMAGINGPYTHONNET-74 Regression: Exif Data is missing exception**

{{< highlight python >}}

import aspose.pycore as pycore
from aspose.imaging import Image, LoadOptions, DataRecoveryMode
from aspose.imaging.fileformats.jpeg import JpegImage

load_options = LoadOptions()
load_options.data_recovery_mode = DataRecoveryMode.CONSISTENT_RECOVER

with pycore.as_of(Image.load("exifdata.jpg", load_options), JpegImage) as image:
    exif_data = image.exif_data
    if exif_data is None:
        raise Exception("ExifData is missing")
    # Do something with it
    bps = exif_data.bits_per_sample

{{< /highlight >}}

