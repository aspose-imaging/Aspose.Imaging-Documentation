---
title: Specify Font Folder for EMF to PNG Conversion
linktitle: Specify Font Folder
type: docs
weight: 30
url: /net/specify-font-folder/
description: Demonstrates how to set custom font folders when converting EMF to PNG using Aspose.Imaging for .NET.
keywords: font settings, emf png, c#
---

# Specify Font Folder for EMF to PNG Conversion

## Introduction
This example shows how to override the default font locations when rasterizing an EMF image to PNG. It is useful when the source EMF references fonts that are not installed on the system.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An EMF file (`Picture1.emf`) in the data directory
- A custom font definition file (e.g., `arialAndTimesAndCourierRegular.xml`)

## Step-by-step Guide
1. Create `EmfRasterizationOptions` and set desired background color.  
2. Create `PngOptions` and assign the rasterization options to it.  
3. Load the EMF image using `Image.Load`.  
4. Reset existing font settings with `FontSettings.Reset()`.  
5. Save the image to PNG using the default font folders.  
6. Retrieve the current font folders, add the path to the custom font file, and apply the updated list with `FontSettings.SetFontsFolders`.  
7. Save the image again to PNG; the output now uses the custom fonts.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "b60525cc0206cb480a642c9e6094f55f" "SpecifyFontFolder.cs" >}}

## See Also
- [Working with EMF Images in Aspose.Imaging](#)
- [Configuring Rasterization Options for Vector Formats](#)
- [Managing Font Settings in Aspose.Imaging](#)
