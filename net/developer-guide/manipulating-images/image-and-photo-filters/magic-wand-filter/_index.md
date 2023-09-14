---
title: Magic Wand tool Image Filter
type: docs
weight: 50
url: /net/developer-guide/manipulating-images/image-and-photo-filters/magic-wand-filter/
description: Magic Wand tool for color area selection. C# code example provided.
keywords: [photo filter, image filter, magic wand, color selection, apply mask]
---

## Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
By using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.magicwand/magicwandtool/">MagicWandTool class</a> from the Aspose.Imaging library, you can select a color area on a loaded image by specifying an arbitrary point within that area using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.magicwand/magicwandsettings/magicwandsettings/">MagicWandSettings</a> parameter. The Magic Wand tool will generate a mask based on color and tone comparisons with the surrounding pixels. You can adjust the mask's coverage by setting the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.magicwand/magicwandsettings/threshold/">Threshold</a> parameter. A higher threshold will result in a larger mask area, potentially including unwanted parts of the image. Conversely, reducing the threshold allows you to create a mask that targets a more specific color area.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Once you've created a mask, you can add additional areas to it using the `Union` method, subtract regions from the existing mask, invert it, and smooth the edges using the `GetFeathered` method. Finally, you can apply the mask to the image and save the resulting image to disk.
</p>

{{< gist "aspose-com-gists" "070228728984c7a658066d52a08044b7" "magic-wand.cs" >}}
