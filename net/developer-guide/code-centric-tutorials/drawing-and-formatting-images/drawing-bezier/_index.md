---
title: Draw a Bézier Curve on an Image using Aspose.Imaging for .NET
linktitle: Drawing Bézier
type: docs
weight: 30
url: /net/drawing-bezier/
description: Demonstrates how to draw a Bézier curve on a bitmap image with Aspose.Imaging for .NET.
keywords: bezier drawing c#
---

# Draw a Bézier Curve on an Image

## Introduction
This example shows how to create a bitmap image and render a Bézier curve on it using the Aspose.Imaging for .NET API. Use it when you need smooth, curved lines for graphics, diagrams, or custom annotations.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- No external image files are required; the example generates the output image programmatically

## Step-by-step Guide
1. **Create a bitmap image** – Set up `BmpOptions` with a 32‑bit color depth and a stream source.
2. **Initialize the `Graphics` object** – Clear the drawing surface with a background color (e.g., yellow).
3. **Configure a `Pen`** – Choose the stroke color (black) and width (3 px) for the Bézier curve.
4. **Define Bézier points** – Specify start, two control, and end coordinates.
5. **Draw the Bézier shape** – Call `Graphics.DrawBezier` with the pen and coordinate values.
6. **Save the image** – Persist the bitmap to the desired location.

## Code Example
The following code demonstrates the complete process:

{{< gist "aspose-imaging-gists" "0b510ff4c8ec003bd0b3cc57bd926d1d" "DrawingBezier.cs" >}}

## See Also
- Drawing straight lines with `Graphics.DrawLine`
- Drawing arcs and circles with `Graphics.DrawArc`
- Exporting images to different formats such as PNG, JPEG, and TIFF
