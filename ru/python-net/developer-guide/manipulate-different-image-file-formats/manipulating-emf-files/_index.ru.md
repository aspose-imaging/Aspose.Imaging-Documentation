---
title: Manipulating EMF Files
type: docs
weight: 60
url: /ru/python-net/manipulating-emf-files/
---

## **Crop EMF Image**
Image cropping usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used for to cut out some portion of an image to increase the focus on a particular area. The **EmfImage** class provides **crop** method that accepts an instance of the **Rectangle** class. You can cut out any portion of an image by providing the desired boundaries to the **Rectangle** object.

The code snippet below demonstrates how to crop any image by Rectangle.

{{< gist "aspose-com-gists" "fa00c266e2a6d57db8a86181eb8fb117" "crop-emf-image.py" >}}
