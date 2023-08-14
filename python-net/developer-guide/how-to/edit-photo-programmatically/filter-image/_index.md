---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/filter-image
linktitle: How to filter an image
title: How to filter an image
description: Filter an image. Apply Rectangular, Sharpen, Motion, Smoothing, Blur, and Median filters.
keywords: [edit a photo, edit an image, filter photo, rectangle filter, sharpen filter, Gauss blur]
---

## How to filter an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The `filter` method supports several filter types such as: `SmallRectangular`, `BigRectangular`, `GaussBlur` and `GaussWiener` to edit a photo or image. Applying rectangle filters will create the effect of looking through a glass placed before a camera through which we can see the picture with different filtered views. The rectangle filter need to set the rectangle dimensions and then apply them to your image by using
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#filter_rectangle_options_25">Filter method</a> with two options. The first option is a Rectangle object and the second is
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.imagefilters.filteroptions/">filter type options</a>. You can apply a filter for a vector image as well, but you need to rasterize it before:
</p>

{{< gist "aspose-com-gists" "ff91f0a36b9bf6eae152d95791eb3bcc" "filter-images.py" >}}

Follow the <a href="https://docs.aspose.com/imaging/python-net/applying-median-and-wiener-filters/">Aspose developer's guide</a> link for more filter examples on Python.
