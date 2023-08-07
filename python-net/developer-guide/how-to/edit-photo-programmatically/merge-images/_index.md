---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/merge-images
linktitle: How to merge images
title: How to merge images
description: Merge images. Combine several images into one. Create a photo collage.
keywords: [merge images, merging images]
---

## How to merge images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Before merging images we need to calculate the total size of the resulting image by summing the total width or height of the images depending on the merge direction. The horizontal direction means that we will sum images widths and we will use direction values 0 in our example, and direction value 1 for the vertical direction. Then we create a new merge image with the calculated dimensions and white background color and place our images to it using <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics/#draw_image_source_image_rect_58">draw_image method</a>.
</p>

{{< gist "aspose-com-gists" "d0728503653a0997a302ddc082221e30" "merge-photos-to-collage.py" >}}
