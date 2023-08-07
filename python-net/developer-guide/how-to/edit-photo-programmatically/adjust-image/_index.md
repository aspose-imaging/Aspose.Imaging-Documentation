---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/adjust-image
linktitle: How to adjust an image
title: How to adjust an image
description: Adjust an image brightness, contrast and gamma coefficient. Gamma corrections.
keywords: [adjust an image, gamma corrections, image brightness, contrast corrections]
---

## How to adjust an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To adjust an image brightness use the
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#adjust_brightness_brightness_1">adjust_brightness method</a> and set a brightness parameter between -255 and 255 to perform corrections. The same you can do with
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#adjust_contrast_contrast_2">adjust_contrast method</a> to make contrast corrections with parameter settings to a range from -100 and 100. If the image has a color hue, you can make gamma corrections by setting the Red, Green and Blue components coefficient or a general gamma coefficient with
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#adjust_contrast_contrast_2">adjust_gamma method</a>:
</p>

{{< gist "aspose-com-gists" "eb0416485d011f42fdaa4412588177a3" "adjust-images.py" >}}

You can find more examples for adjusting images in the <a href="https://docs.aspose.com/imaging/python-net/modifying-images/#adjusting-brightness-contrast-and-gamma">Aspose Developer Guide</a>.
