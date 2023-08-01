---
title: How to filter an image with Aspose.Imaging program library
description: Filter an image. Apply Rectangular, Sharpen, Motion, Smoothing, Blur, and Median filters.
keywords: [edit a photo, edit an image, filter photo, rectangle filter, sharpen filter, Gauss blur]
---

# How to filter an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can select different filter types: `SmallRectangular`, `BigRectangular`, `Sharpen`, `MotionWiener`, `BilateralSmoothing`, `GaussBlur`, `GaussWiener` and `Median` to edit a photo or image. The Rectangle filters create the effect of putting a special glass before a camera through which we can see the picture with different filtered views. To filter a photo with a Rectangle filter just set the rectangle dimensions and then apply them to your image by using <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/filter/">Filter method</a> with two options. The first option is a Rectangle object and the second is <a href="https://reference.aspose.com/imaging/net/aspose.imaging.imagefilters.filteroptions/">filter type options</a>. If you want to apply a filter for a vector image, you need to rasterize it before:
</p>

{% gist aspose-com-gists/a1e5930122ddaf08d6960cb18782d55f filter-images.cs %}
