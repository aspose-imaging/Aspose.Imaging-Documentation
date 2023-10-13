---
title: Remove Watermark Image Filter
type: docs
weight: 50
url: /python-net/developer-guide/manipulating-images/image-and-photo-filters/remove-watermark-filter
description: Aspose.Imaging Remove watermark image filter usage with Python code example provided.
keywords: [image filter, graphic library, remove watermark, watermark removal, paint over, content-aware fill, watermark options, Telea algorithm, painting attempts]
---

## Remove watermark

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To remove watermarks from your photos or images, utilize the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.watermark/watermarkremover/">WatermarkRemover Class</a> from the Aspose.Imaging Python graphic library API. Here's how you can do it:

1. Begin by loading the image that contains the watermark you want to remove.
2. Before applying a method `paint_over` to remove the watermark, you need to define the area where the mark is located on your image.
3. Create a graphic path object with, for example, an elliptical shape figure. The ellipse should be inscribed within a rectangle with coordinates predefined in advance.
4. Create an instance of the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.watermark.options/contentawarefillwatermarkoptions/">ContentAwareFillWatermarkOptions Class</a> and use this ellipse path as an options parameter.
5. The Watermark options support both the `Content-Aware Fill` algorithm and the `Telea` algorithm, allowing you to choose your preferred method.
6. To improve the quality of watermark removal, you have the option to increase the maximal number of painting attempts. However, keep in mind that more attempts will consume more time.

This process enables you to effectively remove watermarks from your images and photos using the Aspose.Imaging Python graphic library.
</p>

Python code example:

{{< gist "aspose-com-gists" "bdeef81eec0653b2096497be988d01ec" "RemoveWatermarkFilter.py" >}}
