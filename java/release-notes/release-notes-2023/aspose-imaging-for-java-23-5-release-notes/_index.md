---
type: docs
weight: '60'
url: /java/aspose-imaging-for-java-23-5-release-notes/
title: Aspose.Imaging for JAVA 23.5 - Release notes
---

## Competitive features:

- **Support of TIFF with Cmyk Alpha color mode**
- **Support of tiled Tiff writing**

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGJAVA-8440 | Support of TIFF with Cmyk Alpha color mode                                                                                                                                  | Feature      |
| IMAGINGJAVA-8427 | Support of tiled Tiff writing                                                                                                                                  | Feature      |
| IMAGINGJAVA-8441 | wk: Converting PNG to TIFF using CMYK colorspace and preserving transparency                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8431 | SVG to PDF: Arrows not rendered correctly                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8426 | Cannot convert the CDR image to JPG                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8395 | Resizing operation is incorrect for GIF animation                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8394 | "Bit depth of 8 bits are supported for RGBA images." exception when rendering PNG file to PNG                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8373 | WMF: Incorrect orientation of wmf rendering                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.5](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-5-release-notes/) version

### Removed APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.5](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-5-release-notes/) version

## Usage Examples:

**IMAGINGJAVA-8441 wk: Converting PNG to TIFF using CMYK colorspace and preserving transparency**

{{< highlight csharp >}}

try (Image png = Image.load("input.png"))
{
	png.save("output.tiff", new TiffOptions(TiffExpectedFormat.TiffLzwCmyka));
}

{{< /highlight >}}

**IMAGINGJAVA-8440 Support of TIFF with Cmyk Alpha color mode**

{{< highlight csharp >}}

try (Image png = Image.load("input.png"))
{
	png.save("output.tiff", new TiffOptions(TiffExpectedFormat.TiffLzwCmyka));
}

{{< /highlight >}}

**IMAGINGJAVA-8431 SVG to PDF: Arrows not rendered correctly**

{{< highlight csharp >}}

try (Image image = Image.load("J1C.svg"))
{
	image.save("J1C.pdf", new PdfOptions());
}

try (Image image = Image.load("J11A.svg"))
{
	image.save("J11A.pdf", new PdfOptions());
}

{{< /highlight >}}

**IMAGINGJAVA-8427 Support of tiled Tiff writing**

{{< highlight csharp >}}

try (TiffImage image = (TiffImage) Image.load("tiled-tiff.tiff"))
{
	TiffFrame page = (TiffFrame) image.getPages()[0];
	if (page.getFrameOptions().isTiled())
	{
		System.out.println("Tiff is tiled");
	}

	image.save("output-tiled.tiff");
}

{{< /highlight >}}

**IMAGINGJAVA-8426 Cannot convert the CDR image to JPG**

{{< highlight csharp >}}

try (Image image = Image.load("Desain Backdrop HUT RI 77 CDR - TUTORiduan.cdr"))
{
	image.save("output.jpeg", new JpegOptions());
}

{{< /highlight >}}

**IMAGINGJAVA-8395 Resizing operation is incorrect for GIF animation**

{{< highlight csharp >}}

List<Integer> resizeTypes = Arrays.asList(
	ResizeType.NearestNeighbourResample,
	ResizeType.AdaptiveResample,
	ResizeType.Bell,
	ResizeType.BilinearResample,
	ResizeType.CatmullRom,
	ResizeType.CubicBSpline,
	ResizeType.CubicConvolution,
	ResizeType.HighQualityResample,
	ResizeType.LanczosResample
);

for (Integer resizeType : resizeTypes)
{
	try (GifImage image = (GifImage) Image.load("test.gif"))
	{
		image.setBackgroundColor(Color.getTransparent());
		image.resizeFullFrame(200, 200, resizeType);
		image.save("test.gif" + "_" +
				ResizeType.getName(ResizeType.class, resizeType) + ".gif");
	}
}

{{< /highlight >}}

**IMAGINGJAVA-8394 "Bit depth of 8 bits are supported for RGBA images." exception when rendering PNG file to PNG**

{{< highlight csharp >}}

try (RasterImage image = (RasterImage) Image.load("image0.png"))
{
    ImageOptionsBase options = image.getOriginalOptions();
    image.save("result.png", options);
}

{{< /highlight >}}

**IMAGINGJAVA-8373 WMF: Incorrect orientation of wmf rendering**

{{< highlight csharp >}}

try (Image image = Image.load("input.wmf"))
{
	PngOptions pngOptions = new PngOptions();
	WmfRasterizationOptions wmf_opt = new WmfRasterizationOptions();
	wmf_opt.setBackgroundColor(Color.getTransparent());
	wmf_opt.setPageHeight(image.getHeight());
	wmf_opt.setPageWidth(image.getWidth());
	pngOptions.setVectorRasterizationOptions(wmf_opt);
	image.save("output.png", pngOptions);
}

{{< /highlight >}}

