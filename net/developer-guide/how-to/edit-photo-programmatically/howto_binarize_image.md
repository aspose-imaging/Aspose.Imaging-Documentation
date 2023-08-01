---
title: How to binarize an image with Aspose.Imaging program library
description: Binarize an image using fixed binarisation method with threshold, method Bradly and Otsu method.
keywords: [binarize an image, binarisation method, grayscaling method, method Bradly, Otsu method]
---

# How to binarize an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To binarize an image with a simple fixed binarisation method <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/binarizefixed/">BinarizeFixed</a>, you need to set only one parameter - a threshold from 0 to 255. All pixels of the image that have an intensity greater than the indicated threshold will be assigned to value 255 (black color), or 0 (white color) otherwise. You can use a more precise grayscaling method `Bradly` <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/binarizebradley/">BinarizeBradley</a> to improve binarization quality. This method calculates the threshold adaptively based on the average intensity estimation of the surrounding area with size `s x s`. In this case, the resulting picture will have more smooth edges. Or you can use `Otsu` method <a href="https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/binarizeotsu/">BinarizeOtsu</a> with automatic threshold:
</p>

{% gist aspose-com-gists/71c0516ed0eaff60994a716cfb062a6a binarize-images.cs %}
