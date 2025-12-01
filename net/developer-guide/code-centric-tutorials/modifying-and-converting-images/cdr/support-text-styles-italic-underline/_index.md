---
title: Support Text Styles: Italic and Underline in CDR Images
linktitle: Italic & Underline Text Styles
type: docs
weight: 30
url: /net/support-text-styles-italic-underline/
description: Demonstrates loading a CDR file and saving it as JPEG while preserving italic and underline text styles.
keywords: cdr conversion italic underline
---

# Support Text Styles: Italic and Underline in CDR Images

## Introduction
This example shows how to work with CorelDRAW (CDR) files using Aspose.Imaging for .NET. It loads a CDR document, ensures that italic and underline text styles are supported, and then saves the image as a JPEG. Use this when you need to convert CDR graphics while retaining text styling.

## Prerequisites
- .NET 9.0 (or later) development environment  
- Aspose.Imaging for .NET library installed  
- A CDR file (e.g., `Test3.cdr`) placed in the example data folder  
- Fonts folder containing the required fonts for proper text rendering  

## Step-by-step Guide
1. **Set the fonts folder** – Configure `FontSettings` to point to the directory that contains the fonts used in the CDR file.  
2. **Locate the input CDR file** – Build the full path to `Test3.cdr` using the provided data directory.  
3. **Load the image** – Use `Image.Load` to read the CDR document into an `Image` object.  
4. **Save as JPEG** – Call `image.Save` with a `.jpg` extension to generate a JPEG representation that keeps italic and underline styles.  
5. **Clean up** – The `using` block disposes of the image automatically, and console messages indicate start and end of the process.

## Code Example
The following code demonstrates the complete example:

{{< gist "aspose-imaging-gists" "ca8032ae3966b7e2b71369ab8225369b" "SupportTextStylesItalicUnderline.cs" >}}

## See Also
- Converting CDR to PNG with Aspose.Imaging  
- Working with fonts in Aspose.Imaging  
- Exporting vector graphics to raster formats
