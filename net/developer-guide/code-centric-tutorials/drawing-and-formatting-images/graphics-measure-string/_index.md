---
title: Measure String Dimensions Using Graphics.MeasureString
linktitle: Graphics Measure String
type: docs
weight: 30
url: /net/graphics-measure-string/
description: Demonstrates how to measure a string’s size with Graphics.MeasureString in Aspose.Imaging for .NET.
keywords: measure string, graphics, aspose imaging
---

# Measure String Dimensions Using Graphics.MeasureString

## Introduction
This example shows how to determine the width and height of a text string when rendered on an image using the `Graphics.MeasureString` method. Use it when you need to layout text precisely or calculate bounding boxes for dynamic content.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library installed
- An input JPEG image file (e.g., `input.jpg`) placed in the example data directory

## Step-by-step Guide
1. Load the background image with `Image.Load`.
2. Create a `Graphics` object from the loaded image.
3. Initialise a `StringFormat` instance (optional formatting).
4. Call `Graphics.MeasureString`, passing the text, a `Font`, an empty `SizeF`, and the `StringFormat`.
5. The method returns a `SizeF` structure containing the measured width and height.

## Code Example
The following code demonstrates the process:

{{< gist "aspose-imaging-gists" "e8e927ea7dd8cd36e08eeebc62d44f39" "GraphicsMeasureString.cs" >}}

## See Also
- **Drawing Text on an Image** – Learn how to render text onto an image using `Graphics.DrawString`.
- **Working with Fonts** – Explore creating and managing font objects in Aspose.Imaging.
- **Image Conversion** – Convert images between formats while preserving drawn content.
