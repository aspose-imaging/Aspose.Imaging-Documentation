---
title: Convert ICO Image to TIFF Format
linktitle: Convert ICO to TIFF
type: docs
weight: 30
url: /net/convert-ico-to-tiff/
description: Converts an ICO image to a TIFF file using Aspose.Imaging for .NET.
keywords: ico tiff conversion
---

# Convert ICO Image to TIFF Format

## Introduction
This example shows how to load an ICO (icon) file and save it as a TIFF image using Aspose.Imaging for .NET. It is useful when you need to work with high‑resolution bitmap representations of icons or integrate ICO assets into workflows that require TIFF format.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0 in the sample project)
- Aspose.Imaging for .NET library
- An ICO file (e.g., `notebook-ico.ico`) placed in the project's data folder

## Step-by-step Guide
1. **Get the data directory** – Resolve the folder that contains the source ICO file.  
2. **Load the ICO image** – Use `Image.Load` to read the icon file into an `Image` object.  
3. **Save as TIFF** – Call `image.Save` with a `TiffOptions` instance to write the image as a TIFF file.  
4. **Clean up (optional)** – Delete the generated TIFF file if it is only needed for demonstration purposes.  
5. **Dispose resources** – The `using` statement ensures the image object is released automatically.

## Code Example
The following C# snippet demonstrates how to perform the conversion:

{{< gist "aspose-imaging-gists" "a60ef7979e72d1fdc26c52a7468d6f76" "ConvertICOToTiff.cs" >}}

## See Also
- **Convert BMP to PNG** – Learn how to change bitmap images to PNG format.  
- **Resize and Rotate Images** – Explore basic image manipulation techniques.  
- **Working with Image Metadata** – Access and modify metadata in various image formats.
