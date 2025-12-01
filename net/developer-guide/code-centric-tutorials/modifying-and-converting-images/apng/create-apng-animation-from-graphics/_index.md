---
title: Create APNG Animation from Graphics
linktitle: APNG Animation from Graphics
type: docs
weight: 30
url: /net/create-apng-animation-from-graphics/
description: Creates an animated APNG image by drawing vector graphics and applying animations using Aspose.Imaging for .NET.
keywords: apng animation c#
---

# Create APNG Animation from Graphics

## Introduction
This example demonstrates how to generate an animated APNG file by programmatically drawing vector graphics (ellipse and line) and applying sequential and parallel animations. Use it when you need to produce lightweight animated images with custom graphics.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- No external assets required; the example creates graphics in code

## Step-by-step Guide
1. **Set up the animation scene** – Define the canvas size and create a `Scene` object to hold graphic objects.
2. **Add graphic objects** – Create an `Ellipse` and a `Line`, configure their visual properties, and add them to the scene.
3. **Define animations** – Use `LinearAnimation`, `Delay`, `SequentialAnimation`, and `ParallelAnimation` to animate the graphics over time.
4. **Configure APNG options** – Create an `ApngOptions` instance with the desired color type and output file path.
5. **Create the APNG image** – Call `Image.Create` with the options, set the default frame time, and play the scene to render frames.
6. **Save and clean up** – Save the animated image and optionally delete the temporary file.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "6f8ce3293dacb72c073b3a78168bd163" "CreateAPNGAnimationFromGraphics.cs" >}}

## See Also
- Converting images to PNG format using Aspose.Imaging
- Creating animated GIFs from bitmap frames
- Working with vector graphics and drawing primitives in Aspose.Imaging
