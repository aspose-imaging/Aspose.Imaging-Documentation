---
type: docs
weight: '90'
url: /ru/java/developer-guide/how-to/edit-photo-programmatically/filter-image
linktitle: How to filter an image
title: How to filter an image
description: Filter an image. Apply Rectangular, Sharpen, Motion, Smoothing, Blur, and Median filters.
keywords: [edit a photo, edit an image, filter photo, rectangle filter, sharpen filter, Gauss blur]
---

## How to filter an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With Aspose.Imaging you can apply filters with different filtering options like: `Sharpen`, `MotionWiener`, `BilateralSmoothing`, `GaussBlur` and `Median` to edit a photo or image. Using a rectangle filter creates the effect of a special glass put before a camera through which we can see the picture. To apply a rectangle filter an image passes the `Rectangle` object as a first parameter of the
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#filter-com.aspose.imaging.Rectangle-com.aspose.imaging.imagefilters.filteroptions.FilterOptionsBase-">Filter method</a>  and the second parameter a
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging.imagefilters.filteroptions/">filter type options</a>. Applying the filter to a vector image is also possible, in this case, the vector image needs to be rasterized before that:
</p>

{{< gist "aspose-com-gists" "62fbf25d357f9630abcc20d79d5947b2" "filter-images.java" >}}

More Java code examples you can find in the <a href="https://docs.aspose.com/imaging/ru/java/applying-median-and-wiener-filters/">Aspose documentation</a>.
