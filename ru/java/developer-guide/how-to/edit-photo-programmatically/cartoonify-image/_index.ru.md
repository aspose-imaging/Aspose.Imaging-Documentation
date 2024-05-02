---
type: docs
weight: '90'
url: /ru/java/developer-guide/how-to/edit-photo-programmatically/cartoonify-image
linktitle: How to cartoonify an image
title: How to cartoonify an image
description: Cartoonify an image. Convert photo to cartoon style.
keywords: [cartoonify an image, cartoon style, convolution filter, select outlines]
---

## How to cartoonify an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Creating a cartoon-style image from your photo involves various image editing methods. You need to detect areas with similar colors by applying a convolution filter and blurring the image with
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#filter-com.aspose.imaging.Rectangle-com.aspose.imaging.imagefilters.filteroptions.FilterOptionsBase-">Filter method</a>, also you need to select outlines and binarize outlines with threshold `30` by using
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#binarizeFixed-byte-">BinarizeFixed method</a>, use image masking with
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.masking/imagemasking/#applyMask-com.aspose.imaging.RasterImage-com.aspose.imaging.RasterImage-com.aspose.imaging.masking.options.MaskingOptions-">ApplyMask method</a>:
</p>

{{< gist "aspose-com-gists" "e8d356ec157169159aba5650730a227f" "cartoonify-images.java" >}}
