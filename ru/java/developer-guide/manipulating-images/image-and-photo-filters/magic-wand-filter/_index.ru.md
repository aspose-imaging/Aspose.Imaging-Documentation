---
title: Magic Wand tool Image Filter
type: docs
weight: 50
url: /ru/java/developer-guide/manipulating-images/image-and-photo-filters/magic-wand-filter/
description: Magic Wand tool for color area selection. Java code example provided.
keywords: [photo filter, image filter, magic wand, color selection, masked region, apply mask, color comparison]
---

## Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To create a mask corresponding to a specific color area, you can take advantage of the new Magic Wand tool supported by the Aspose.Imaging library since the 23.8 release. Here's how you can use it:

1. Begin by loading an image or photo.
2. Create a new mask by using the `select` method of the <a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.magicwand/magicwandtool/">MagicWandTool</a> class.
3. To specify the color region you want to mask, provide the coordinates of a point inside that region using the <a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.magicwand/magicwandsettings/">MagicWandSettings</a> object.
4. The method will automatically select an area around the specified point with similar colors and tones using color comparison.
5. You can adjust the size of the masked region by setting the `setThreshold` parameter, which accepts values between 0 and 100. This parameter acts as a tolerance level for comparing pixel colors.
6. Additionally, you have the option to combine the existing mask with a new one, subtract one mask from another, or invert the selection.
7. To achieve smoother edges for the resulting mask, you can apply the `Feathering` method, specifying the desired `setSize` parameter in pixels.
8. Finally, apply the mask to the image and save the final image in a format supported by the Aspose.Imaging library.

This process allows you to precisely select and mask specific color areas within your images or photos using the Magic Wand tool in the Aspose.Imaging library.
</p>

{{< gist "aspose-com-gists" "af8fa5e0ddd6a6b3c728ef316f1fc318" "magic-wand.java" >}}
