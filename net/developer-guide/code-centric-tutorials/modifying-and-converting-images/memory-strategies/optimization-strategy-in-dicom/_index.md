---
title: Optimize DICOM Image Memory Strategy
linktitle: Optimization Strategy in DICOM
type: docs
weight: 30
url: /net/optimization-strategy-in-dicom/
description: Demonstrates how to use a custom memory strategy when creating and modifying DICOM images with Aspose.Imaging for .NET.
keywords: dicom, memory strategy, c#
---

# Optimize DICOM Image Memory Strategy

## Introduction
This example shows how to create a DICOM image using a memory‑based source, draw vector graphics on it, and manage multiple pages with brightness adjustments. Use it when you need fine‑grained control over memory usage while working with DICOM files in .NET.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- No additional input files are required; the example generates an image entirely in memory.

## Step-by-step Guide
1. **Create a DICOM image** using `Image.Create` with `DicomOptions` that points to a `MemoryStream` source.  
2. **Draw vector graphics** on the first page using `Graphics` and various brushes.  
3. **Extract pixel data** from the first page with `LoadArgb32Pixels`.  
4. **Add additional pages** after the first one, applying incremental brightness changes via `AdjustBrightness`.  
5. **Insert pages before the first page**, applying inverse brightness changes to create brighter pages.  
6. **Save the multi‑page DICOM image** to a temporary file and clean up.

## Code Example
The following snippet contains the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "d08c5b3a19109a3112a6f53c0da995d0" "OptimizationStrategyInDicom.cs" >}}

## See Also
- Working with DICOM images in Aspose.Imaging  
- Adding and inserting pages in multi‑page images  
- Adjusting image brightness and contrast programmatically
