---
title: Create an Image Using a Stream with Aspose.Imaging for .NET
linktitle: Create Image from Stream
type: docs
weight: 30
url: /net/creating-image-using-stream/
description: Demonstrates how to create a BMP image from a stream using Aspose.Imaging for .NET.
keywords: stream image c#
---

# Create an Image Using a Stream

## Introduction
This example shows how to generate a BMP image directly from a .NET `Stream` object with Aspose.Imaging.  
Use it when you need to create images in memory or write them to custom storage without first saving to a file.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Access to a writable folder for reading/writing sample files used by the example

## Step-by-step Guide
1. **Prepare the output stream** – Open a `FileStream` (or any `Stream`) where the BMP will be written.  
2. **Configure BMP options** – Create `BmpOptions`, set required properties like `BitsPerPixel`, and assign the stream via `StreamSource`.  
3. **Create the image** – Call `Image.Create` with the configured options and desired dimensions (e.g., 500 × 500).  
4. **Perform any processing** – Optionally manipulate the image (draw, rescale, etc.) before saving.  
5. **Save the image** – Use `image.Save` to write the generated bitmap to the target path.  
6. **Dispose resources** – Ensure the `Stream` and `Image` objects are properly disposed (the `using` statement handles this automatically).

## Code Example
Below is the complete code for this scenario:

{{< gist "aspose-imaging-gists" "bd642d04d1564bfb86ff33c57ee9ebc6" "CreatingImageUsingStream.cs" >}}

## See Also
- **Saving Images in Different Formats** – Learn how to save images as JPEG, PNG, TIFF, etc.  
- **Working with Image Streams** – Explore reading images from streams and processing them in memory.  
- **Advanced BMP Options** – Dive deeper into BMP-specific settings such as color depth and compression.
