---
title: Save EMF Graphics Using Aspose.Imaging for .NET
linktitle: Save EMF Graphics
type: docs
weight: 30
url: /net/save-emf-graphics/
description: Demonstrates how to draw vector graphics and save them as an EMF file with Aspose.Imaging.
keywords: emf, graphics, c#
---

# Save EMF Graphics

## Introduction
This example demonstrates how to create vector graphics with **EmfRecorderGraphics2D**, draw text using custom fonts and styles, and save the result as an EMF (Enhanced Metafile) image. Use this approach when you need scalable, high‑resolution graphics for printing or further vector‑based processing.

## Prerequisites
- .NET 9.0 (or any supported .NET version)
- Aspose.Imaging for .NET library
- No external input files are required; the example generates the EMF file in the output directory.

## Step-by-step Guide
1. **Set up the data directory** – Retrieve the location where the generated EMF file will be saved.  
2. **Create an `EmfRecorderGraphics2D` instance** – Define the drawing canvas size and resolution.  
3. **Draw text with different fonts and styles** – Use `Font` objects to render strings in bold, underline, italic, and strike‑out styles.  
4. **Finalize the drawing** – Call `EndRecording()` to obtain an `EmfImage` containing the recorded graphics.  
5. **Save the EMF image** – Store the resulting file using `EmfOptions`.  

## Code Example
The following code snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "dc6c139db8760615fbd022299d16cfb5" "SaveEmfGraphics.cs" >}}

## See Also
- **Converting EMF to other formats** – Learn how to convert the generated EMF file to PNG, JPEG, or PDF.  
- **Loading and editing existing EMF files** – Explore how to open an existing EMF image, modify its content, and save changes.  
- **Working with other vector graphics formats** – Understand how Aspose.Imaging handles SVG, WMF, and other vector formats.
