---
type: docs
weight: '90'
url: /ru/java/developer-guide/how-to/edit-photo-programmatically/binarize-image
linktitle: How to binarize an image
title: How to binarize an image
description: Binarize an image using fixed binarisation method with threshold, method Bradly and Otsu method.
keywords: [binarize an image, binarisation method, grayscaling method, method Bradly, Otsu method]
---

## How to binarize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The simple binarization method with a fixed threshold
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#binarizeFixed-byte-">BinarizeFixed</a> is using only one parameter - a threshold with value from 0 to 255. All pixels in this case that have an intensity greater than the defined threshold will be set as a black color, or if less than the threshold, then to a white color. You can use a more precise binarize method `Bradly`
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#binarizeBradley-double-">BinarizeBradley</a> to improve binarization quality. Method `Bradly` use the threshold as an average estimation intensity of the surrounding area with size `s x s`. In this case, the resulting picture will have smooth edges. Also, you can use `Otsu` method
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/rasterimage/#binarizeOtsu--">BinarizeOtsu</a> with automatic threshold:
</p>

{{< gist "aspose-com-gists" "daac19b481878f17e5e6caadd16bb490" "binarize-images.java" >}}
