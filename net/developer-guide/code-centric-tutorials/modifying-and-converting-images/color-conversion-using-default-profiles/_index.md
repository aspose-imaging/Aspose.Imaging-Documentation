---
title: Color Conversion Using Default Profiles
linktitle: Color Conversion
type: docs
weight: 30
url: /net/color-conversion-using-default-profiles/
description: Demonstrates how to convert an image’s colors using default RGB and CMYK profiles with Aspose.Imaging for .NET.
keywords: color-conversion c# aspose-imaging
---

# Color Conversion Using Default Profiles

## Introduction
This example shows how to apply default RGB and CMYK color profiles to a JPEG image and save the result. Use it when you need to ensure consistent color representation across different devices or output media.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- Input files: a JPEG image (e.g., `aspose-logo_tn.jpg`), `rgb.icc`, and `cmyk.icc` profile files

## Step-by-step Guide
1. Retrieve the data directory that contains the source image and profile files.  
2. Load the JPEG image using `Image.Load`.  
3. Open the RGB and CMYK ICC profile files as `StreamSource` objects.  
4. Assign the streams to `DestinationRgbColorProfile` and `DestinationCmykColorProfile` of the image.  
5. Save the image to a new file, which now embeds the specified color profiles.  

## Code Example
The complete source code is shown below:

{{< gist "aspose-imaging-gists" "69e4a50c07be0bfccefd2d09587d676b" "ColorConversionUsingDefaultProfiles.cs" >}}

## See Also
- Working with Color Profiles in Aspose.Imaging
- Converting Image Formats with Aspose.Imaging
- Manipulating JPEG Images in C#
