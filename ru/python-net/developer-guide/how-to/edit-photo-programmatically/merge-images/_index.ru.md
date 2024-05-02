---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/edit-photo-programmatically/merge-images
linktitle: How to merge images
title: How to merge images
description: Merge images. Combine several images into one. Create a photo collage.
keywords: [merge images, merging images]
---

## How to merge images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
If you would like to merge images into one, you need to calculate the total size of the resulting image by summing the total width or height of the images depending on the merge direction. In the case of the horizontal direction, we will sum images widths and use a direction value equal to `0` in our example, and sum heights for the vertical direction with the value of `1`. Next, create a new merge image with the calculated dimensions and desired background color and place the images to it using <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/graphics/#draw_image_source_image_rect_58">draw_image method</a>.
</p>

{{< gist "aspose-com-gists" "d0728503653a0997a302ddc082221e30" "merge-photos-to-collage.py" >}}
