---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically/remove-background
linktitle: How to remove background from an image
title: How to remove background from an image
description: Removing photo background. Change image background color.
keywords: [remove background, photo background change, feathering radius, auto masking graph cut]
---

## How to remove background from an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To remove photo background, you can use the
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.masking.options/automaskinggraphcutoptions/">AutoMaskingGraphCutOptions class</a> with automatically calculated strokes and set property by using
<a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.masking.options/graphcutmaskingoptions/#setFeatheringRadius-int-">setFeatheringRadius method</a> to smooth and blur the cutting edge. The feathering radius is calculated as 1/500 of the image dimension. You need to set a new color, when you've removed the background, in the Java code example below we use transparent pixels. So, the same procedure can be used for photo background changing.
</p>

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-feathering.java" >}}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a more detailed description with Java code examples please follow the link to <a href="https://docs.aspose.com/imaging/java/removing-background-from-images/">Aspose Developer's guide</a>.
</p>
