---
title: Support GIF Frame Duration and Number of Cycles
linktitle: Support GIF Frame Duration
type: docs
weight: 30
url: /net/support-gif-frame-duration-and-number-of-cycles/
description: Demonstrates how to adjust GIF frame duration and specify the number of animation cycles using Aspose.Imaging for .NET.
keywords: gif duration loops c#
---

# Support GIF Frame Duration and Number of Cycles

## Introduction
This example shows how to modify the duration of individual frames in a GIF image and set the total number of animation loops (cycles). Use it when you need precise control over GIF playback timing or want the animation to repeat a specific number of times.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample GIF file (e.g., `ezgif.com-gif-maker(1)___.gif`) placed in the example data folder

## Step-by-step Guide
1. Load the source GIF using `Image.Load`.
2. Adjust the overall frame time with `SetFrameTime`.
3. Change the duration of a specific frame via the `GifFrameBlock.FrameTime` property.
4. Save the modified image, specifying the desired number of loops through `GifOptions.LoopsCount`.
5. (Optional) Delete the generated output file after verification.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "85d6b75b15f184dbbafea53d0c5a1b75" "SupportGifFrameDurationAndNumberOfCycles.cs" >}}

## See Also
- Changing GIF Frame Properties
- Converting Images to GIF Format
- Working with Animated Images in Aspose.Imaging
