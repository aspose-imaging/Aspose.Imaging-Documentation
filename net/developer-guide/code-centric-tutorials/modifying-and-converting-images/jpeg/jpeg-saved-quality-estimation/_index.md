---
title: Estimate Saved JPEG Quality
linktitle: JPEG Saved Quality
type: docs
weight: 30
url: /net/jpeg-saved-quality-estimation/
description: Demonstrates how to check the saved quality of a JPEG image using Aspose.Imaging for .NET.
keywords: jpeg quality c#
---

# Estimate Saved JPEG Quality

## Introduction
This example shows how to determine whether a JPEG image has been saved with a quality setting different from the default (75). Use it when you need to validate or enforce image quality standards in your .NET applications.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample JPEG file (e.g., `test.jpg`) placed in the data directory used by the examples

## Step-by-step Guide
1. Load the JPEG image using `Image.Load`.
2. Cast the loaded image to `JpegImage` to access JPEG‑specific properties.
3. Retrieve the `Quality` value from `JpegOptions`.
4. Compare the retrieved quality with the default value (75) to determine if a non‑default quality was used.
5. Output the result or take appropriate action based on the quality check.

## Code Example
The following code snippet demonstrates the process:

{{< gist "aspose-imaging-gists" "5b0daf51663be837c74c91d1b1f58088" "JpegSavedQualityEstimation.cs" >}}

## See Also
- [Working with JPEG Metadata](/net/working-with-jpeg-metadata/)
- [Changing JPEG Compression Quality](/net/changing-jpeg-compression-quality/)
- [Saving Images in Different Formats](/net/saving-images-in-different-formats/)
