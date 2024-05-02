---
type: docs
weight: '90'
url: /ru/java/developer-guide/how-to/edit-photo-programmatically/adjust-image
linktitle: How to adjust an image
title: How to adjust an image
description: Adjust an image brightness, contrast and gamma coefficient. Gamma corrections.
keywords: [adjust an image, gamma corrections, image brightness, contrast corrections]
---

## How to adjust an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can adjust an image brightness by using the
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#adjustBrightness-int-">AdjustBrightness method</a> and set a brightness parameter in a range from -255 to 255 for performing corrections. The same you can do with
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#adjustContrast-float-">AdjustContrast method</a> to make contrast corrections with parameter settings to a range from -100 and 100. If the image has a color component domination, you can make gamma corrections by setting the Red, Green and Blue components coefficient using
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#adjustGamma-float-float-float-">AdjustGamma method</a>:
</p>

{{< gist "aspose-com-gists" "822bcdd56fb7d62b05d9d0ad94cfba29" "adjust-images.java" >}}
