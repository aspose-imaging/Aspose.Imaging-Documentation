---
title: Unify Usage of Common Operations in Image Processing
linktitle: Unify Usage of Common Operations
type: docs
weight: 40
url: /net/unify-usage-of-common-operations/
description: Demonstrates unified handling of common image operations across different formats using Aspose.Imaging for .NET.
keywords: image processing, aspose imaging, c#
---

# Unify Usage of Common Operations in Image Processing

## Introduction
This example shows how to apply common image operations—such as cropping and saving—in a unified way, regardless of whether the source file is an OpenDocument format or another raster format. It is useful when you need a single workflow that adapts to different image types.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- An input image file (e.g., `test.cdr`) placed in the example data directory

## Step-by-step Guide
1. **Load the image** using `Image.Load`.
2. **Determine the image type** (e.g., `OdImage` for OpenDocument formats).
3. **Apply cropping** with coordinates that differ based on the image type.
4. **Save the result** as a PNG, configuring rasterization options to preserve vector quality.
5. **Clean up** by deleting the temporary output file.

## Code Example
The following code illustrates these steps:

{{< gist "aspose-imaging-gists" "039a67757720f77448f639d50a201d33" "UnifyUsageOfCommonOperations.cs" >}}

## See Also
- Converting images between formats with Aspose.Imaging
- Applying image transformations such as rotation and scaling
- Working with vector rasterization options for high‑quality output
