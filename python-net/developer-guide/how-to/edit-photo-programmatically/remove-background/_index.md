---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically/remove-background
linktitle: How to remove background from an image
title: How to remove background from an image
description: Removing photo background. Change an image's background color.
keywords: [remove background, photo background change, feathering radius, auto masking graph cut]
---

## How to remove background from an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the example below, there are several methods are used to remove the image background. The method with manual processing rectangles required indicating rectangles with objects in advance and also marking background and foreground points. Using the auto-processing method with assumed objects you need to specify the detected object type (e.g. `HUMAN`) and the rectangle area where the object is located. In the other automatic methods, we just use the class <a href="https://reference.aspose.com/imaging/python-net/aspose.imaging.masking.options/automaskinggraphcutoptions/">AutoMaskingGraphCutOptions class</a> with automatically calculated strokes and set `FeatheringRadius` property to smooth and blur the cutting edge. After removing a background we need to set the color to replace it. The same procedure can be used for photo background change.
</p>

{{< gist "aspose-com-gists" "291380aac991e0869dbabba3e60f5225" "remove-change-background-generic-examples.py" >}}
