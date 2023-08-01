---
title: How to merge images with Aspose.Imaging program library
description: Merge images. Combine several images into one. Create a photo collage.
keywords: [merge images, merging images]
---

# How to merge images with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Before merging images we need to calculate the total size of the resulting image by summing the total width or height of the images depending on the merge direction. The horizontal direction means that we will sum images widths and we will use direction values 0 in our example, and direction value 1 for the vertical direction. Then we create a new merge image with the calculated dimensions and white background color, and place our images to it using <a href="https://reference.aspose.com/imaging/net/aspose.imaging/graphics/drawimage/">DrawImage method</a>.
</p>

{% gist aspose-com-gists/c3b1f39eaf550446e244e071b29d5191 merge-photos-to-collage.cs %}
