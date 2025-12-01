---
title: Using TextRenderingHint to Control Text Rendering While Converting Images
linktitle: Support of TextRenderingHint
type: docs
weight: 30
url: /net/support-of-text-rendering-hint/
description: Demonstrates how to apply TextRenderingHint when converting vector images to PNG.
keywords: text rendering hint c#
---

# Using TextRenderingHint to Control Text Rendering While Converting Images

## Introduction
This example shows how to use the **TextRenderingHint** enumeration to influence the quality of text rendering when rasterizing various vector image formats to PNG. It is useful when you need crisp or anti‑aliased text output in the resulting bitmap.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample vector files: `TextHintTest.cdr`, `TextHintTest.cmx`, `TextHintTest.emf`, `TextHintTest.wmf`, `TextHintTest.odg`, `TextHintTest.svg`

## Step-by-step Guide
1. **Set up the data directory** where the sample vector files are located.  
2. **Create an array of file names** for the vector formats you want to process.  
3. **Define the list of TextRenderingHint values** you wish to test (e.g., AntiAlias, ClearTypeGridFit, etc.).  
4. **Load each vector file** using `Image.Load`.  
5. **Determine the appropriate rasterization options** based on the image type (Cdr, Cmx, Emf, Wmf, Odg, Svg).  
6. **Assign the current TextRenderingHint** to the rasterization options.  
7. **Save the rasterized image** as PNG with the configured `VectorRasterizationOptions`.  
8. **Repeat** the process for every hint and every input file, producing a set of output PNGs that illustrate the visual impact of each rendering hint.

## Code Example
The following snippet contains the complete implementation of the workflow described above.

{{< gist "aspose-imaging-gists" "651e6957984503ee4babcbc2e629f680" "SupportOfTextRenderingHint.cs" >}}

## See Also
- Rasterizing Vector Images with Aspose.Imaging
- Converting Images to Different Formats Using Aspose.Imaging
- Working with Image Options and Export Settings
