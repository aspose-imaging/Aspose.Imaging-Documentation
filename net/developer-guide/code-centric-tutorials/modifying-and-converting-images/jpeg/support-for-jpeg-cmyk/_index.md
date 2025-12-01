---
title: Support for JPEG CMYK Using Aspose.Imaging for .NET
linktitle: Support for JPEG CMYK
type: docs
weight: 30
url: /net/support-for-jpeg-cmyk/
description: Demonstrates how to save and load CMYK JPEG‑LS images with Aspose.Imaging for .NET.
keywords: jpeg cmyk .net
---

# Support for JPEG CMYK Images

## Introduction
This example shows how to work with CMYK JPEG‑LS images using Aspose.Imaging for .NET. It covers saving an image in the CMYK color space with JPEG‑LS compression and then loading it back for further processing.

## Prerequisites
- .NET runtime (compatible with your project, e.g., .NET 6 or later)  
- Aspose.Imaging for .NET library installed via NuGet or manual reference  
- A source JPEG file (e.g., `056.jpg`) placed in the project’s data folder

## Step-by-step Guide
1. **Prepare the data directory** – Obtain the path to the folder containing the source JPEG file.  
2. **Create a memory stream** – This will hold the CMYK JPEG‑LS data temporarily.  
3. **Load the source JPEG image** – Use `JpegImage` to open the original file.  
4. **Configure JPEG options**:  
   - Set `ColorType` to `JpegCompressionColorMode.Cmyk`.  
   - Set `CompressionType` to `JpegCompressionMode.JpegLs`.  
   - (Optional) Leave color profiles as `null` to use default profiles.  
5. **Save the image to the memory stream** with the configured options.  
6. **Reset the stream position** to zero before reading.  
7. **Load the CMYK JPEG‑LS image from the stream** using `JpegImage`.  
8. **Export the loaded image** to a desired format, such as PNG, with `PngOptions`.  
9. **Dispose of the memory stream** to release resources.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "393dee65ac08eb35e1b621ee176e94cf" "SupportForJPEG-LSWithCMYK.cs" >}}

## See Also
- Converting JPEG to PNG with Aspose.Imaging  
- Working with JPEG options and compression modes  
- Processing CMYK images in .NET applications
