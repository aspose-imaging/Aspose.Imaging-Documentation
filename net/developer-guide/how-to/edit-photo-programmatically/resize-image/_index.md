---
type: docs
weight: '90'
url: /net/developer-guide/how-to/edit-photo-programmatically/resize-image
linktitle: Resize an image
title: How to resize an image
description: Resize an image. Change photos height and width. Sizing photos proportionally.
keywords: [resize an image, resizing an image, resizing photos, photo sizing, picture resizer]
---

# How to resize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For resizing an image, we are using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/image/load">method Load</a> of the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/image/">class Image</a> to load an image into a cache memory. Then we apply <a href="https://reference.aspose.com/imaging/net/aspose.imaging/image/resize/">Resize method</a> to the image with a new size by specifying desired height and width `300x300` in pixels and save the result to a new file.
</p>

Example C# code:
{{< gist "aspose-com-gists" "7ee37a401e37790396ad9f4cde87d446" "simple-resizing-image.cs" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Additionally, you can make photo sizing proportionally the picture width or height and specify the resizing type by selecting `ResizeType.LanczosResample` parameter:
</p>

{{< gist "aspose-com-gists" "7ee37a401e37790396ad9f4cde87d446" "resize-image-with-resize-type-enumeration.cs" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
There are several Resize types available for resizing photos. Please see the link to the table which describes the <a href="https://docs.aspose.com/imaging/net/crop-rotate-and-resize-images/#resizing-images--resizetype-enumeration">resize type parameters</a>.
</p>
