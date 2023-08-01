---
title: How to remove background from an image with Aspose.Imaging program library
description: Removing photo background. Change image background color.
keywords: [remove background, photo background change, feathering radius, auto masking graph cut]
---

# How to remove background from an image with Aspose.Imaging program library

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the example below, to carefully remove background, we use the class <a href="https://reference.aspose.com/imaging/net/aspose.imaging.masking.options/automaskinggraphcutoptions/">AutoMaskingGraphCutOptions class</a> with automatically calculated strokes and set <a href="https://reference.aspose.com/imaging/net/aspose.imaging.masking.options/graphcutmaskingoptions/featheringradius/">FeatheringRadius property</a> to smooth and blur the cutting edge. The feathering radius is calculated as 1/500 of the image dimension. After removing a background we need to set the color to replace it, so we use transparent pixels in this case. The same procedure we can use for photo background change.
</p>

{% gist aspose-com-gists/cd4fed97fcdfa3055fbffc65e5298664 graph-cut-feathering.cs %}

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
For a more detailed description with examples of how to remove background please follow the <a href="https://docs.aspose.com/imaging/net/removing-background-from-images/">Aspose removing background documentation</a>.
</p>
