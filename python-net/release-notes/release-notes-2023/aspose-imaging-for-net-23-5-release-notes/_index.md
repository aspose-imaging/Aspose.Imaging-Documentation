---
type: docs
weight: '60'
url: /python-net/aspose-imaging-for-python-net-23-5-release-notes/
title: Aspose.Imaging for Python via .NET 23.5 - Release notes
---

## Competitive features:

- **Support of TIFF with Cmyk Alpha color mode**
- **Support of tiled Tiff writing**

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGNET-5986 | Support of tiled Tiff writing                                                                                                                                  | Feature      |
| IMAGINGNET-6191 | WMF: Incorrect orientation of wmf rendering                                                                                                                                  | Enhancement      |
| IMAGINGNET-6181 | SVG to PDF: Arrows not rendered correctly                                                                                                                                  | Enhancement      |
| IMAGINGNET-6102 | Support of TIFF with Cmyk Alpha color mode                                                                                                                                  | Enhancement      |
| IMAGINGNET-6101 | wk: Converting PNG to TIFF using CMYK colorspace and preserving transparency                                                                                                                                  | Enhancement      |
| IMAGINGNET-5802 | Cannot convert the CDR image to JPG                                                                                                                                  | Enhancement      |
| IMAGINGNET-4605 | "Bit depth of 8 bits are supported for RGBA images." exception when rendering PNG file to PNG                                                                                                                                  | Enhancement      |
| IMAGINGNET-4600 | Resizing operation is incorrect for GIF animation                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.5](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-5-release-notes/) version

### Removed APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.5](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-5-release-notes/) version

## Usage Examples:

**IMAGINGNET-6191 WMF: Incorrect orientation of wmf rendering**

{{< highlight python >}}

with Image.load("input.wmf") as image:
	pngOptions = PngOptions()
	wmf_options = WmfRasterizationOptions()
	wmf_options.background_color = Color.transparent
	wmf_options.page_width = image.width
	wmf_options.page_height = image.height
	pngOptions.vector_rasterization_options = wmf_options
	image.save("output.png", pngOptions)

{{< /highlight >}}

**IMAGINGNET-6181 SVG to PDF: Arrows not rendered correctly**

{{< highlight python >}}

with Image.load("D:\\J1C.svg")) as image:
	pdfOptions = new PdfOptions()
	image.save("D:\\J1C.pdf", pdfOptions)

with Image.load("D:\\J11A.svg")) as image:
	pdfOptions = new PdfOptions()
	image.save("D:\\J11A.pdf", pdfOptions)

{{< /highlight >}}

**IMAGINGNET-6102 Support of TIFF with Cmyk Alpha color mode**

{{< highlight python >}}

with Image.load("input.png") as png:
	png.save("output.tiff", new TiffOptions(TiffExpectedFormat.TiffLzwCmyka))

{{< /highlight >}}

**IMAGINGNET-6101 wk: Converting PNG to TIFF using CMYK colorspace and preserving transparency**

{{< highlight python >}}

with Image.load("input.png") as png:
	png.save("output.tiff", new TiffOptions(TiffExpectedFormat.TiffLzwCmyka))

{{< /highlight >}}

**IMAGINGNET-5986 Support of tiled Tiff writing**

{{< highlight python >}}

with aspose.pycore.as_of(Image.load("tiled-tiff.tiff"), TiffImage) as image:
	page = aspose.pycore.as_of(image.pages[0], TiffFrame)
	if page.frame_options.is_tiled:
		print("Tiff is tiled")

	image.save("output-tiled.tiff")

{{< /highlight >}}

**IMAGINGNET-5802 Cannot convert the CDR image to JPG**

{{< highlight python >}}

with Image.load("Desain Backdrop HUT RI 77 CDR - TUTORiduan.cdr") as image:
	image.save("output.jpeg", new JpegOptions())

{{< /highlight >}}

**IMAGINGNET-4605 "Bit depth of 8 bits are supported for RGBA images." exception when rendering PNG file to PNG**

{{< highlight python >}}

with aspose.pycore.as_of(Image.load("image0.png"), RasterImage) as image:
    options = image.get_original_options()
    image.save("result.png", options)

{{< /highlight >}}

**IMAGINGNET-4600 Resizing operation is incorrect for GIF animation**

{{< highlight python >}}

resizeTypes = [ResizeType.NEAREST_NEIGHBOUR_RESAMPLE,
			   ResizeType.ADAPTIVE_RESAMPLE,
			   ResizeType.BELL,
			   ResizeType.BILINEAR_RESAMPLE,
			   ResizeType.CATMULL_ROM,
			   ResizeType.CUBIC_B_SPLINE,
			   ResizeType.CUBIC_CONVOLUTION,
			   ResizeType.HIGH_QUALITY_RESAMPLE,
			   ResizeType.LANCZOS_RESAMPLE]

for resize_type in resizeTypes:
    with aspose.pycore.as_of(Image.load("test.gif"), GifImage) as image:
        image.background_color = Color.transparent
        image.resize_full_frame(200, 200, resize_type)
        image.save("test" + "_" + resize_type.name + ".gif")

{{< /highlight >}}
