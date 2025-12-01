---
title: Convert DIB to PNG Using Aspose.Imaging
linktitle: Support of DIB
type: docs
weight: 40
url: /net/support-of-dib/
description: Demonstrates loading a DIB image and converting it to PNG with Aspose.Imaging for .NET.
keywords: dib conversion c#
---

# Convert DIB to PNG Using Aspose.Imaging

## Introduction
- This example shows how to load a Device Independent Bitmap (DIB) image and save it as a PNG file.  
- Use it when you need to work with legacy DIB/BMP files and convert them to modern formats for further processing or display.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample DIB file (`sample.dib`) placed in the data directory used by the example

## Step-by-step Guide
1. **Prepare the data directory** – Determine the folder that contains the input DIB file.  
2. **Load the DIB image** – Use `Image.Load` to read the `sample.dib` file into an `Image` object.  
3. **Inspect the format (optional)** – Access `image.FileFormat` to verify that the file is recognized as a BMP/DIB format.  
4. **Save as PNG** – Call `image.Save` with a new file name (`sample.png`) and a `PngOptions` instance to convert and write the image in PNG format.  

## Code Example
The following C# code demonstrates the process:

{{< gist "aspose-imaging-gists" "ed2868615632a35f0e1195e1981cb44d" "SupportOfDIB.cs" >}}

## See Also
- Converting images to other formats with Aspose.Imaging  
- Working with BMP and DIB files in Aspose.Imaging  
- Using image options such as `PngOptions` and `JpegOptions`
