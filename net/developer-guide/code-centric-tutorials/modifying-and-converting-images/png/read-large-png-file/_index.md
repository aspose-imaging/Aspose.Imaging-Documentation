---
title: Read Large PNG File and Convert to JPEG
linktitle: Read Large PNG
type: docs
weight: 30
url: /net/read-large-png-file/
description: Demonstrates how to load a large PNG image with Aspose.Imaging for .NET and save it as a JPEG.
keywords: png convert c#
---

# Read Large PNG File and Convert to JPEG

## Introduction
This example shows how to efficiently load a large PNG image using Aspose.Imaging for .NET and convert it to a JPEG format. It is useful when working with high‑resolution PNG files that need to be reduced in size or changed to a more widely supported format.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A large PNG file (e.g., `halfGigImage.png`) placed in the example data folder

## Step-by-step Guide
1. **Set up the data directory** – Retrieve the path where the sample PNG file resides.  
2. **Load the large PNG image** – Use `Image.Load` to read the PNG file without loading the entire image into memory at once.  
3. **Convert and save as JPEG** – Create a `JpegOptions` instance and call `image.Save` to write the image to a JPEG file.  
4. **Dispose resources** – The `using` block ensures the image is properly disposed after processing.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "f4f075b3fb10b6e8f919556d1aa0e621" "ReadLargePNGFile.cs" >}}

## See Also
- [Loading and Saving Images with Aspose.Imaging](#)
- [Working with Large Images in .NET](#)
- [Converting PNG to JPEG Using Aspose.Imaging](#)
