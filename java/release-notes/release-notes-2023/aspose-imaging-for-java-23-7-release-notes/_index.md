---
type: docs
weight: '60'
url: /java/aspose-imaging-for-java-23-7-release-notes/
title: Aspose.Imaging for JAVA 23.7 - Release notes
---

## Competitive features:

- **Add alpha blending feature for RasterImage**

| **Key**         | **Summary**                                                                                                                                                              | **Category** |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| IMAGINGJAVA-8477 | UnIfy naming conventions                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8476 | Synchronize use of Pages and format specific collections for multi page images                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8475 | Add alpha blending feature for RasterImage                                                                                                                                  | Enhancement      |
| IMAGINGJAVA-8470 | EMF export error                                                                                                                                  | Enhancement      |

## Public API changes:

### Added APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.7](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-7-release-notes/) version

### Removed APIs:

Please see corresponding cumulative [API changes for Aspose.Imaging for .NET 23.7](https://docs.aspose.com/imaging/net/aspose-imaging-for-net-23-7-release-notes/) version

## Usage Examples:

**IMAGINGJAVA-8477 UnIfy naming conventions**

{{< highlight csharp >}}

long format = com.aspose.imaging.FileFormat.Unknown;
System.out.print(format);

{{< /highlight >}}

**IMAGINGJAVA-8476 Synchronize use of Pages and format specific collections for multi page images**

{{< highlight csharp >}}

long[] fileFormats = {FileFormat.Tiff, FileFormat.Gif, FileFormat.Dicom};
for (long fileFormat : fileFormats)
{
	String fileName = getTestFilePath(fileFormat);
	try (Image image = Image.load(fileName))
	{
		int expectPageCount = ((IMultipageImage) image).getPageCount() + 1;
		if (fileFormat == FileFormat.Tiff)
		{
			TiffImage tiffImage = (TiffImage) image;
			this.checkPages(tiffImage.getFrames(), tiffImage.getPages());
			tiffImage.removeFrame(1);
			tiffImage.addFrame(tiffImage.getFrames()[0]);
			tiffImage.insertFrame(0, tiffImage.getFrames()[0]);
			this.checkPages(tiffImage.getFrames(), tiffImage.getPages());
		}
		else if (fileFormat == FileFormat.Gif)
		{
			GifImage gifImage = (GifImage) image;
			Image[] images = this.readImageBlocksFromGif(gifImage);
			this.checkPages(images, gifImage.getPages());
			IGifBlock block = null;
			final IGifBlock[] gifImageBlocks = gifImage.getBlocks();
			for (IGifBlock gifImageBlock : gifImageBlocks)
			{
				if (gifImageBlock instanceof Image)
				{
					block = gifImageBlock;
					break;
				}
			}

			assert block != null;

			gifImage.removeBlock(block);
			gifImage.addBlock(new GifGraphicsControlBlock());
			gifImage.addBlock(block);

			gifImage.insertBlock(0, block);
			gifImage.insertBlock(0, new GifGraphicsControlBlock());
			images = readImageBlocksFromGif(gifImage);
			this.checkPages(images, gifImage.getPages());
		}
		else if (fileFormat == FileFormat.Dicom)
		{
			DicomImage dicomImage = (DicomImage) image;
			this.checkPages(dicomImage.getDicomPages(), dicomImage.getPages());
			dicomImage.removePage(0);
			dicomImage.insertPage(0);
			dicomImage.addPage(dicomImage.getDicomPages()[0]);
			this.checkPages(dicomImage.getDicomPages(), dicomImage.getPages());
		}

		assert expectPageCount == ((IMultipageImage) image).getPageCount();
	}
}

{{< /highlight >}}

**IMAGINGJAVA-8475 Add alpha blending feature for RasterImage**

{{< highlight csharp >}}

try(RasterImage background = (RasterImage) Image.load("background.webp"))
{
	try(RasterImage overlay = (RasterImage)Image.load("logo.png"))
	{
		Point center = new Point((background.getWidth() - overlay.getWidth()) / 2, 
								 (background.getHeight() - overlay.getHeight()) / 2);
		background.blend(center, overlay, overlay.getBounds(), (byte) 127);

		background.save("blended.webp");
	}
}

{{< /highlight >}}

**IMAGINGJAVA-8470 EMF export error**

{{< highlight csharp >}}

try (Image image = Image.load("33.emf"))
{
	image.save("emf-to-png.png");
}

{{< /highlight >}}

