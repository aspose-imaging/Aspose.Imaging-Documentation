---
title: Color Conversion Using ICC Profiles (C#)
linktitle: Color Conversion (ICC Profiles)
type: docs
weight: 30
url: /net/color-conversion-using-icc-profiles/
description: Demonstrates how to apply ICC color profiles to a JPEG image using Aspose.Imaging for .NET.
keywords: icc color-profile c# imaging
---

# Convert Image Colors Using ICC Profiles

## Introduction
This example shows how to load ICC color profiles and apply them to an image with Aspose.Imaging for .NET. Use it when you need to ensure accurate color representation across different devices or color spaces.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample JPEG image (`aspose-logo_tn.jpg`)
- ICC profile files (`rgb.icc` and `cmyk.icc`)

## Step-by-step Guide
1. **Load the source image** – Open the JPEG image using `Image.Load`.
2. **Read ICC profiles** – Create `StreamSource` objects for the RGB and CMYK ICC files.
3. **Assign profiles to the image** – Set `RgbColorProfile` and `CmykColorProfile` properties on the image object.
4. **Access pixel data** – Optionally call `LoadPixels` to work with the image pixels after the profiles are applied.
5. **Dispose resources** – Use a `using` block or manually dispose of the image to release file handles.

## Code Example
The following snippet demonstrates the process:

{{< gist "aspose-imaging-gists" "7ad99e72d4e4f1adcc0b1970404fa080" "ColorConversionUsingICCProfiles.cs" >}}

## See Also
- Applying Color Profiles with Aspose.Imaging
- Converting Image Formats Using Aspose.Imaging
- Working with JPEG Images in Aspose.Imaging
