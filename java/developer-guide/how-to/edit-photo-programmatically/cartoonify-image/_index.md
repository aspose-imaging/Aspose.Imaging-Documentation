---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/cartoonify-image
linktitle: How to cartoonify an image
title: How to cartoonify an image
description: Cartoonify an image. Convert photo to cartoon style.
keywords: [cartoonify an image, cartoon style, convolution filter, select outlines]
---

## How to cartoonify an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To convert an image to a cartoon style we will use various image editing methods. Detecting areas with similar colors is done by applying a convolution filter to blur the image with
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#filter-com.aspose.imaging.Rectangle-com.aspose.imaging.imagefilters.filteroptions.FilterOptionsBase-">Filter method</a>, selecting outlines, binarize outlines with threshold 30 using
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#binarizeFixed-byte-">BinarizeFixed method</a>, and masking the image with
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.masking/imagemasking/#applyMask-com.aspose.imaging.RasterImage-com.aspose.imaging.RasterImage-com.aspose.imaging.masking.options.MaskingOptions-">ApplyMask method</a>:
</p>

{{< gist "aspose-com-gists" "e8d356ec157169159aba5650730a227f" "cartoonify-images.java" >}}
