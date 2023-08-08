---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/resize-image
linktitle: How to resize an image
title: How to resize an image
description: Resize an image. Change photos height and width. Sizing photos proportionally.
keywords: [resize an image, resizing an image, resizing photos, photo sizing, picture resizer]
---

## How to resize an image

### Resize with resizing type

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For resizing an image, we are using the
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/image/#load_file_path_21">method Load</a> of the
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/image/">class Image</a> to load an image into cache memory. Then we apply
<a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/image/#resize_new_width_new_height_28">Resize method</a> to the image with a new size by specifying desired height and width `300x300` in pixels and specify the resizing type by selecting `ResizeType.LANCZOS_RESAMPLE` parameter.
</p>

Example Python code:
{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-with-resize-type.py" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
There are several Resize types available for resizing photos. Please see the link to the table which describes the <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging/resizetype/">resize type parameters</a>.
</p>


### Proportional resizing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Additionally, you can make photo sizing proportionally the picture width or height:
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-image-proportionally.py" >}}
