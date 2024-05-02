---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/edit-photo-programmatically/resize-image
linktitle: How to resize an image
title: How to resize an image
description: Resize an image. Change photos height and width. Sizing photos proportionally.
keywords: [resize an image, resizing an image, resizing photos, photo sizing, picture resizer]
---

## How to resize an image

### Resize with resizing type

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To resize an image, load your image with
<a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/#load_file_path_21">method Load</a> of the Python
<a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/">class Image</a>. Then you can apply the
<a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/image/#resize_new_width_new_height_28">Resize method</a> with specifying height and width (`300x300` px)  and selecting the resizing type `LANCZOS_RESAMPLE`.
</p>

Example Python code:
{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-with-resize-type.py" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Several resize types are available for resizing photos. Please refer to the table with descriptions of <a href="https://reference.aspose.com/imaging/ru/python-net/aspose.imaging/resizetype/">Resize type parameters</a>.
</p>


### Proportional resizing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Also, you can use proportional resizing and specify only desired picture width or height:
</p>

{{< gist "aspose-com-gists" "e3ab4246a7061ee32df42c74051bdaff" "resize-image-proportionally.py" >}}
