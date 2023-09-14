---
title: Magic Wand tool Image Filter
type: docs
weight: 50
url: /python-net/developer-guide/manipulating-images/image-and-photo-filters/magic-wand-filter
description: Magic Wand tool for color area selection. Python code example provided.
keywords: [image effect, image filter, magic wand, color selection, color comparison, color tolerance, select mask, apply mask]
---

## Magic Wand tool

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can select a specific color region on a loaded image using the Magic Wand tool, which has been available since Aspose.Imaging library version 23.8. The <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.magicwand/magicwandtool/">MagicWandTool Class</a> supports several useful methods, including select, union, invert, and subtract for manipulating masks. To select a color area, you need to specify a point with X and Y coordinates inside that area. The Magic Wand tool then uses the color and tone of that pixel as a reference and compares it with the surrounding pixels. If the select method finds these pixels to be similar, it adds them to the resulting area. Consequently, the method returns a mask representing the selected color area. An additional parameter, `threshold`, in the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.magicwand/magicwandsettings/">MagicWandSettings</a> object sets the tolerance level for pixel color comparison. A higher threshold value increases color tolerance, leading to a wider selection of the color area.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Moreover, you have the flexibility to perform various operations on masks. You can invert the selected mask, combine it with another mask using the union method, or subtract one mask from another. To refine the mask's appearance, you can utilize the `Feathering` method to smooth the mask edges, with the option to specify the desired feathering size in pixels. Once you're satisfied with the mask, apply it to the image to achieve the desired image effect.
</p>

{{< gist "aspose-com-gists" "bc2a6d39abf8d6e186411a663b1b1224" "magic-wand.py" >}}
