---
title: Create GraphicsPath from TIFF Path Resources and Vice Versa
linktitle: GraphicsPath from TIFF
type: docs
weight: 30
url: /net/create-graphics-path-from-path-tiff-resources-and-vice-versa/
description: Demonstrates how to convert TIFF path resources to a GraphicsPath and back using Aspose.Imaging for .NET.
keywords: tiff graphicspath c#
---

# Create GraphicsPath from TIFF Path Resources and Vice Versa

## Introduction
This example shows how to extract path resources from a TIFF image, convert them into a `GraphicsPath` for drawing, and then convert a custom `GraphicsPath` back into TIFF path resources. Use it when you need to manipulate vector information embedded in TIFF files or create new vector data for a TIFF image.

## Prerequisites
- .NET 6.0 or higher (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- Sample TIFF file named **Bottle.tif** placed in the data directory used by the examples

## Step-by-step Guide
1. Load the source TIFF image using `Image.Load`.
2. Retrieve the image’s active frame and its `PathResources`.
3. Convert the `PathResources` to a `GraphicsPath` with `PathResourceConverter.ToGraphicsPath`.
4. Draw on the image using the created `GraphicsPath` (e.g., a red border).
5. Save the modified image.
6. Create a new `GraphicsPath` manually (e.g., a rectangular figure made of `BezierShape` objects).
7. Convert this custom `GraphicsPath` back to TIFF `PathResources` via `PathResourceConverter.FromGraphicsPath`.
8. Assign the new `PathResources` to the image’s active frame and save the result.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "5a72f6f89dd7b0bb991e7fff99efb437" "CreateGraphicsPathFromPathTiffResourcesAndViceVersa.cs" >}}

## See Also
- **Working with TIFF images** – general operations on TIFF files using Aspose.Imaging
- **Drawing shapes with Graphics** – how to use the `Graphics` class for vector drawing
- **Converting between image formats** – converting TIFF to other raster formats with Aspose.Imaging
