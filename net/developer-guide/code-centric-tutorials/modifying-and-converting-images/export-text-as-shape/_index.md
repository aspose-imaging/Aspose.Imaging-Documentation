---
title: Export Text as Shape
linktitle: Export Text as Shape
type: docs
weight: 30
url: /net/export-text-as-shape/
description: Shows how to export text as vector shapes when converting EMF to SVG using Aspose.Imaging for .NET.
keywords: export text shape, svg, c#
---

# Export Text as Shape

## Introduction
This example demonstrates how to export the textual content of an EMF image as vector shapes when saving it to SVG format. Use this technique when you need the text to be preserved as scalable shapes rather than font references, ensuring consistent rendering across devices.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample EMF file (e.g., `Picture1.emf`) placed in the example’s data directory

## Step-by-step Guide
1. Load the source EMF image using `Image.Load`.
2. Configure `EmfRasterizationOptions` to define background color and page dimensions.
3. Save the image to SVG with `TextAsShapes` set to **true** to convert text into shapes.
4. Save the image again with `TextAsShapes` set to **false** to retain text as font references (optional for comparison).

## Code Example
The following snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "b84ec9a95a83dd4d7d4e1a87e2d6fe45" "ExportTextAsShape.cs" >}}

## See Also
- [Converting EMF to PNG with Aspose.Imaging](#)
- [Working with Vector Rasterization Options](#)
- [Saving Images with Custom SVG Options](#)
