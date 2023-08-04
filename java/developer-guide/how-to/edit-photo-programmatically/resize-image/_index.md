---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/resize-image
linktitle: How to resize an image
title: How to resize an image
description: Resize an image. Change photos height and width. Sizing photos proportionally.
keywords: [resize an image, resizing an image, resizing photos, photo sizing, picture resizer]
---

## How to resize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For resizing an image, we are using the 
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/#load-java.lang.String-">method Load</a> of the 
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/">class Image</a> to load an image into a cache memory. Then we apply 
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/#resize-int-int-">Resize method</a> to the image with a new size by specifying desired height and width `300x300` in pixels and save the result to a new file.
</p>

Example Java code:
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-SimpleResizing-SimpleResizing.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Additionally, you can make photo sizing proportionally the picture width or height and specify the resizing type by selecting `ResizeType.LanczosResample` parameter:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ResizeImageWidthwithResizeTypeEnumeration-ResizeImageWidthwithResizeTypeEnumeration.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
There are several Resize types available for resizing photos. Please see the link to the table which describes the <a href="https://docs.aspose.com/imaging/java/crop-rotate-and-resize-images/#resizing-images--resizetype-enumeration">resize type parameters</a>.
</p>
