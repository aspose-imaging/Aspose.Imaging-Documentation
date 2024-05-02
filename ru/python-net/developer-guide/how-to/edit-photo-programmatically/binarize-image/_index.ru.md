---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/edit-photo-programmatically/binarize-image
linktitle: How to binarize an image
title: How to binarize an image
description: Binarize an image using fixed binarisation method with threshold, method Bradly and Otsu method.
keywords: [binarize an image, binarisation method, grayscaling method, method Bradly, Otsu method]
---

## How to binarize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To transform an image to a black-and-white binary form you can use the binarization method with fixed threshold
<a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#binarize_bradley_brightness_difference_5">BinarizeFixed</a>, so, in this case, you need to indicate a threshold in a range of 0 and 255. All pixels of the image that have an intensity greater than the selected threshold will be assigned to value 255 (black color), or 0 (white color) otherwise. The more precise method is a `Bradly` method
<a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/rasterimage/#binarize_bradley_brightness_difference_5">BinarizeBradley</a> is used to improve binarization quality. The method calculates the threshold adaptively based on the average intensity estimation of the surrounding area with size `s x s`. The resulting picture will have more smooth edges in this case. Also, you can use Otsu method (`BinarizeOtsu`) with an automatic threshold.
</p>

{{< gist "aspose-com-gists" "3fa6b0222e82664ed1216a1a2f5d3663" "binarize-images.py" >}}
