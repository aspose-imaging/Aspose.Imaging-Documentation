---
title: Remove Watermark Image Filter
type: docs
weight: 50
url: /net/developer-guide/manipulating-images/image-and-photo-filters/remove-watermark-filter/
description: Using Aspose.Imaging graphic library with Remove watermark image filter. C# code example provided.
keywords: [graphic library, image filter, remove watermark, watermark remover, watermark mask, watermark options, graphic path, content-aware fill, Telea algorithm, maximal painting attempts, paint over]
---

## Remove watermark

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Starting from Aspose.Imaging graphic library version 23.9, we have introduced a new feature: the Remove Watermark image filter. This filter managed through the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark/watermarkremover/">WatermarkRemover class</a>, allows you to manipulate watermark signatures on your images or photos.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the following C# code example, we illustrate how to use this feature. We begin by loading a PNG image that contains a watermark. In this specific case, the watermark is situated within a circular area. To specify the watermark's location on the image, we create a corresponding graphic path. We refer to this path object as a 'mask' and include an ellipse shape in this path. The coordinates for the ellipse inscribed within the rectangle are pre-determined.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
After creating the watermark mask with the ellipse shape, we utilize the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark/watermarkremover/paintover/">WatermarkRemover.PaintOver method</a> to process the PNG image using <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark.options/">Watermark.Options</a>. Additionally, we employ <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark.options/contentawarefillwatermarkoptions/">ContentAwareFillWatermarkOptions</a> and configure the <a href="https://reference.aspose.com/imaging/net/aspose.imaging.watermark.options/contentawarefillwatermarkoptions/maxpaintingattempts/">MaxPaintingAttempts property</a> to be 1. This means that the 'Content-Aware Fill' algorithm will make a maximum of one painting attempt and choose the best fill option. It's important to note that more attempts generally yield better results, but they also consume more time. Alternatively, you can opt for the 'Telea' algorithm, which is also available as an option.
</p>

C# code example:
