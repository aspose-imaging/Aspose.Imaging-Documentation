---
title: Convert DNG to JPEG with Aspose.Imaging for .NET
linktitle: Convert DNG to JPEG
type: docs
weight: 30
url: /net/converting-dng-to-jpg/
description: Demonstrates how to convert a DNG image to JPEG using Aspose.Imaging for .NET.
keywords: dng jpg conversion c#
---

# Convert DNG to JPEG

## Introduction
This example shows how to load a DNG (Digital Negative) file and save it as a JPEG image using Aspose.Imaging for .NET. Use it when you need to convert raw camera files to a widely supported format for sharing or further processing.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DNG source file and a writable folder for the resulting JPEG

## Step-by-step Guide
1. Specify the full paths for the source DNG file and the destination JPEG file.  
2. Load the DNG image using `Image.Load`, casting it to `DngImage`.  
3. Create a `JpegOptions` instance to define JPEG-specific settings (defaults are sufficient for a basic conversion).  
4. Call `Save` on the `DngImage` instance, passing the destination path and the `JpegOptions`.  
5. Dispose of the image object (the `using` statement handles this automatically).

## Code Example
The following code snippet demonstrates the conversion process:

{{< gist "aspose-imaging-gists" "66c9eecc56a847b286215fc22d1a8ac0" "ConvertingDNGToJPG.cs" >}}

## See Also
- **Convert RAW to PNG** – Learn how to convert other raw image formats to PNG.  
- **Apply JPEG compression settings** – Customize JPEG quality and other options during saving.  
- **Batch processing images** – Process multiple images in a single operation with Aspose.Imaging.
