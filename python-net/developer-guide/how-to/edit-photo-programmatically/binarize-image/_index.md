---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/binarize-image
linktitle: How to binarize an image
title: How to binarize an image
description: Binarize an image using fixed binarisation method with threshold, method Bradly and Otsu method.
keywords: [binarize an image, binarisation method, grayscaling method, method Bradly, Otsu method]
---

## How to binarize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To binarize an image with a simple fixed binarisation method
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#binarize_bradley_brightness_difference_5">BinarizeFixed</a>, you need to set only one parameter - a threshold from 0 to 255. All pixels of the image that have an intensity greater than the indicated threshold will be assigned to value 255 (black color), or 0 (white color) otherwise. You can use a more precise grayscaling method `Bradly`
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/rasterimage/#binarize_bradley_brightness_difference_5">BinarizeBradley</a> to improve binarization quality. This method calculates the threshold adaptively based on the average intensity estimation of the surrounding area with size `s x s`. In this case, the resulting picture will have more smooth edges. Alternatively, you can use Otsu method (`BinarizeOtsu`) with an automatic threshold.
</p>

{{< gist "aspose-com-gists" "3fa6b0222e82664ed1216a1a2f5d3663" "binarize-images.py" >}}
