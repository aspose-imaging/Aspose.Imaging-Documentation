---
title: How to cartoonify an image with Aspose.Imaging program library
description: Cartoonify an image. Convert photo to cartoon style.
keywords: [cartoonify an image, cartoon style, convolution filter, select outlines]
---

# How to cartoonify an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To convert an image to a cartoon style we will use various image editing methods. Detecting areas with similar colors is done by applying a convolution filter to blur the image with <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/filter/">Filter method</a>, selecting outlines, binarize outlines with threshold 30 using <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/binarizefixed/">BinarizeFixed method</a>, and masking the image with <a href="https://reference.aspose.com/imaging/net/aspose.imaging.masking/imagemasking/applymask/">ApplyMask method</a>:
</p>

{% gist aspose-com-gists/06ef86978a9c043ccf04b5c6fd292b4c cartoonify-images.cs %}
