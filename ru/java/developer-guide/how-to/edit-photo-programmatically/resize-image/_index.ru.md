---
type: docs
weight: '90'
url: /ru/java/developer-guide/how-to/edit-photo-programmatically/resize-image
linktitle: How to resize an image
title: How to resize an image
description: Resize an image. Change photos height and width. Sizing photos proportionally.
keywords: [resize an image, resizing an image, resizing photos, photo sizing, picture resizer]
---

## How to resize an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Before editing an image you need to load your image into cache memory using
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/image/#load-java.lang.String-">method Load</a> of the Java
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/image/">class Image</a>. Next, apply 
<a href="https://reference.aspose.com/imaging/ru/java/com.aspose.imaging/image/#resize-int-int-">Resize method</a> to the image with a new size by selecting new height and width `300x300` in pixels and finally save the result to a file.
</p>

Example Java code:
{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-SimpleResizing-SimpleResizing.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can make image sizing proportionally the image width or height by specifying the resizing type by selecting `ResizeType.LanczosResample` parameter:
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ResizeImageWidthwithResizeTypeEnumeration-ResizeImageWidthwithResizeTypeEnumeration.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The available resize types are listed in the table of the <a href="https://docs.aspose.com/imaging/ru/java/crop-rotate-and-resize-images/#resizing-images--resizetype-enumeration">Resize type parameters</a>.
</p>
