---
title: Saving SVG with Fonts Using Aspose.Imaging for .NET
linktitle: Save SVG with Fonts
type: docs
weight: 30
url: /net/saving-svg-with-fonts/
description: Demonstrates how to save SVG files with embedded or external fonts using Aspose.Imaging for .NET.
keywords: svg fonts c#
---

# Save SVG with Fonts Using Aspose.Imaging

## Introduction
This example illustrates how to read SVG files that contain either embedded or exported fonts, save them while preserving the font resources, and optionally export the SVG to PDF. Use it when you need precise control over font handling in SVG output.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A set of SVG test files (e.g., `EmbeddedFonts.svg`, `ExportedFonts.svg`, `mysvg.svg`) located in a source folder such as `D:\FontTests`

## Step-by-step Guide
1. **Prepare output folders** – Ensure the output and font sub‑folders exist; the example creates them automatically if missing.  
2. **Read an SVG file** – Load the SVG using `Image.Load`.  
3. **Configure rasterization options** – Set up `SvgRasterizationOptions` (or `EmfRasterizationOptions` for saving) to define page size and background color.  
4. **Choose font storage mode** – Decide whether fonts should be embedded directly in the SVG (`Embedded`) or stored as external font files (`Stream`).  
5. **Save the SVG** – Call `image.Save` with `SvgOptions`, providing a custom `SvgCallbackFontTest` to handle font resource callbacks.  
6. **Validate external fonts** – When using the `Stream` mode, verify that the expected number of font files has been generated.  
7. **Export to PDF (optional)** – Use `PdfOptions` with `SvgRasterizationOptions` to convert the SVG to a PDF document.

## Code Example
The following snippet shows the complete workflow described above:

{{< gist "aspose-imaging-gists" "ad8caa11f1ba7296a760e349254ec630" "SavingSVGWithFonts.cs" >}}

## See Also
- Working with SVG rasterization options  
- Exporting SVG to PDF with Aspose.Imaging  
- Managing font resources in vector graphics
