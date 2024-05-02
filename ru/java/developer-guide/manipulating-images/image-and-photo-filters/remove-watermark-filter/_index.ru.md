---
title: Remove Watermark Image Filter
type: docs
weight: 50
url: /ru/java/developer-guide/manipulating-images/image-and-photo-filters/remove-watermark-filter/
description: Remove watermark image filter usage with Java code example provided.
keywords: [graphic library, image filter, watermark remover, remove watermark, watermark options, content-aware fill, painting attempts, java class, paint over method]
---

## Remove watermark

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can utilize the `Remove Watermark` image filter using the Aspos.Imaging graphic library for Java to eliminate unwanted marks from your images and photos. This library features the <a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.watermark/watermarkremover/">WatermarkRemover</a> Java class, which includes the `paintOver` method for manipulating watermarks.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the example below, we start by loading a PNG image with a watermark. We proceed to create a graphic path object that defines the location and shape of the watermark. In our case, the watermark is enclosed within an elliptical shape, and the coordinates for this ellipse need to be defined before image processing. To remove the watermark, we pass the loaded image to the `paintOver` method, along with an object containing <a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.watermark.options/watermarkoptions/">WatermarkOptions</a>. In this case, we utilize the `Content-Aware Fill` algorithm option with the ellipse shape path as a mask parameter. Additionally, we set the maximum painting attempts to 4. This implies that the algorithm will generate 4 images and select the best result.
</p>

Java code example:

{{< gist "aspose-com-gists" "3899d43a1ee9b6ada0bf45acacef8412" "RemoveWatermarkFilter.java" >}}
