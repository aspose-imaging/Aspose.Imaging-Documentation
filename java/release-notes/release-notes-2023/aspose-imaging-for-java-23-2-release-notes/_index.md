---
type: docs
weight: '60'
url: /java/aspose-imaging-for-java-23-2-release-notes/
title: Aspose.Imaging for JAVA 23.2 - Release notes
---

## Competitive features:

- **Keep transparency, when indexing Png images**

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGJAVA-8339 | Keep transparency, when indexing Png images                                                                                                                                  | Feature      |
| IMAGINGJAVA-8344 | SVG export issue                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8343 | Image export failed when converting DCM to PNG                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8342 | Convert TIFF to PDF loses color                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8341 | ICO to PDF export bug                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8331 | ImageExtensions.toJava takes too long to convert                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.2](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-2-release-notes/) version

### Removed APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.2](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-2-release-notes/) version

## Usage Examples:

**IMAGINGJAVA-8344 SVG export issue**

{{< highlight csharp >}}

try (Image image = Image.load("input.svg"))
{
	image.save("output.svg", new SvgOptions()
	{{
		setCallback(new KeepEmbeddedFonts());
	}});
}

static class KeepEmbeddedFonts extends SvgResourceKeeperCallback
{
	@Override
	public void onFontResourceReady(FontStoringArgs args)
	{
		args.setFontStoreType(FontStoreType.Embedded);
	}
}

{{< /highlight >}}

**IMAGINGJAVA-8343 Image export failed when converting DCM to PNG**

{{< highlight csharp >}}

try (Image image = Image.load("input.dcm"))
{
    image.save("output.png", new PngOptions());
}

{{< /highlight >}}

**IMAGINGJAVA-8342 Convert TIFF to PDF loses color**

{{< highlight csharp >}}

try (Image image = Image.load("1.tiff"))
{
	PdfOptions options = new PdfOptions();
	options.setFullFrame(true);
	options.setUseOriginalImageResolution(true);
	options.setPdfCoreOptions(new PdfCoreOptions()
			{{
				setCompression(PdfImageCompressionOptions.None);
			}});

	image.save("1.tiff.pdf", options);
}

{{< /highlight >}}

**IMAGINGJAVA-8341 ICO to PDF export bug**

{{< highlight csharp >}}

try (Image ico = Image.load("aladin-d.ico"))
{
    ico.save("aladin-d.pdf", new PdfOptions());
}

{{< /highlight >}}

**IMAGINGJAVA-8339 Keep transparency, when indexing Png images**

{{< highlight csharp >}}

try (RasterImage image = (RasterImage)Image.load("input_png_with_alpha.png"))
{
    PngOptions options = new PngOptions()
    {{
        setCompressionLevel(9);
        setColorType(PngColorType.IndexedColor);
        setPalette(ColorPaletteHelper.getCloseTransparentImagePalette(image, 256));
        setFilterType(PngFilterType.Avg);
    }};

    image.save("input_png_with_alpha_out.png", options);
}

{{< /highlight >}}

**IMAGINGJAVA-8331 ImageExtensions.toJava takes too long to convert**

{{< highlight csharp >}}

RasterImage image = (RasterImage) Image.load("D:\\Temp\\IMAGINGJAVA-8331\\mainImage.jpg");
try
{
	BufferedImage picture = com.aspose.imaging.extensions.ImageExtensions.toJava(image);
}
finally
{
	image.close();
}

{{< /highlight >}}

