---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/filter-image
linktitle: How to filter an image
title: How to filter an image
description: Filter an image. Apply Rectangular, Sharpen, Motion, Smoothing, Blur, and Median filters.
keywords: [edit a photo, edit an image, filter photo, rectangle filter, sharpen filter, Gauss blur]
---

## How to filter an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can select different filter types: `SmallRectangular`, `BigRectangular`, `Sharpen`, `MotionWiener`, `BilateralSmoothing`, `GaussBlur`, `GaussWiener` and `Median` to edit a photo or image. The Rectangle filters create the effect of putting a special glass before a camera through which we can see the picture with different filtered views. To filter a photo with a Rectangle filter just set the rectangle dimensions and then apply them to your image by using
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#filter-com.aspose.imaging.Rectangle-com.aspose.imaging.imagefilters.filteroptions.FilterOptionsBase-">Filter method</a> with two options. The first option is a Rectangle object and the second is
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.imagefilters.filteroptions/">filter type options</a>. If you want to apply a filter for a vector image, you need to rasterize it before:
</p>

{{< gist "aspose-com-gists" "62fbf25d357f9630abcc20d79d5947b2" "filter-images.java" >}}

Please follow the link to find more <a href="https://docs.aspose.com/imaging/java/applying-median-and-wiener-filters/">Filter examples</a>.
