---
title: Add a Signature to an Image using Aspose.Imaging for .NET
linktitle: Add Signature to Image
type: docs
weight: 30
url: /net/add-signature-to-image/
description: Demonstrates how to overlay a signature graphic onto an image and save the result.
keywords: signature, image, c#
---

# Add a Signature to an Image

## Introduction
This example shows how to load a primary image, overlay a signature graphic onto it, and save the combined result. Use it when you need to embed watermarks, logos, or any custom signature onto images programmatically.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample image files: `SampleTiff1.tiff` (base image) and `signature.gif` (signature graphic)

## Step-by-step Guide
1. Initialize the data directory that contains the source images.  
2. Load the primary image using `Image.Load`.  
3. Load the signature graphic as a second `Image` instance.  
4. Create a `Graphics` object linked to the primary image.  
5. Draw the signature image onto the primary image at the desired location (bottom‑right corner in this example).  
6. Save the modified image to the desired format, e.g., PNG, using `PngOptions`.  

## Code Example
The following snippet contains the complete source code for this scenario:

{{< gist "aspose-imaging-gists" "5c89fa8e08f1b5ca6d28199545ad3a89" "AddSignatureToImage.cs" >}}

## See Also
- Adding a watermark to an image
- Converting image formats with Aspose.Imaging
- Rotating and scaling images programmatically
