---
title: Convert MetaFiles to SVG with Embedded or Exported Images
linktitle: MetaFiles to SVG
type: docs
weight: 30
url: /net/meta-files-as-svg/
description: Learn how to convert MetaFiles to SVG format, choosing between embedding images or exporting them as separate resources using Aspose.Imaging for .NET.
keywords: svg conversion c#
---

# Convert MetaFiles to SVG with Embedded or Exported Images

## Introduction
This example demonstrates how to convert MetaFile formats (such as EMF) into SVG documents using Aspose.Imaging for .NET.  
It shows two approaches: embedding rasterized images directly into the SVG file or exporting them as separate image resources.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A source MetaFile (e.g., `auto.svg` derived from an EMF file) placed in a local folder
- Write permissions for the output directory where SVG and image resources will be saved

## Step-by-step Guide
1. **Prepare the working directories** – define source, output, and image sub‑folders.  
2. **Load the MetaFile** – use `Image.Load` to read the source file.  
3. **Configure rasterization options** – create an `EmfRasterizationOptions` instance with the desired page size and background color.  
4. **Set SVG options** – attach the rasterization options and a callback (`SvgCallbackImageTest`) that determines whether images are embedded or saved externally.  
5. **Save the SVG** – call `image.Save` with the configured `SvgOptions`.  
6. **(Optional) Verify exported images** – when using external resources, enumerate the generated files and compare them against the expected list.

## Code Example
The following Gist contains the full implementation of the described workflow:

{{< gist "aspose-imaging-gists" "2034ab2ade3896a93d5bda81b653a6ab" "MetaFilesAsSVG.cs" >}}

## See Also
- **Export MetaFile to PNG** – converting MetaFiles to raster formats.  
- **Working with SVG callbacks** – customizing how resources are handled during SVG generation.  
- **Embedding images in PDF** – similar techniques for PDF output with Aspose.Imaging.
