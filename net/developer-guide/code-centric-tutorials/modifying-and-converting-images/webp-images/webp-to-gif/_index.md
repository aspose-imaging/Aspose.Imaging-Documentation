---
title: Convert WebP Animation to GIF using Aspose.Imaging for .NET
linktitle: WebP to GIF
type: docs
weight: 30
url: /net/webp-to-gif/
description: Demonstrates converting an animated WebP file to a GIF with Aspose.Imaging for .NET.
keywords: webp gif c#
---

# Convert WebP Animation to GIF

## Introduction
This example shows how to convert an animated WebP image into a GIF file using Aspose.Imaging for .NET. It is useful when you need to provide GIF support for platforms that do not handle WebP animation natively.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample file: `Animation.webp` (included in the Aspose.Imaging example data)

## Step-by-step Guide
1. Retrieve the path to the directory containing the sample WebP file.
2. Load the WebP image using `Image.Load` and cast it to `WebPImage`.
3. Create a `GifOptions` instance to specify GIF-specific settings.
4. Save the loaded image as a GIF by calling `image.Save` with the desired output path and the `GifOptions`.
5. (Optional) Delete the generated GIF file to clean up after execution.

## Code Example
The following code demonstrates the complete conversion process:

{{< gist "aspose-imaging-gists" "836560ae97b8902ec53e2f796d94b3f7" "WebPToGifExample.cs" >}}

## See Also
- Converting PNG to GIF with Aspose.Imaging
- Working with animated images in Aspose.Imaging
- Optimizing image size using Aspose.Imaging compression features
