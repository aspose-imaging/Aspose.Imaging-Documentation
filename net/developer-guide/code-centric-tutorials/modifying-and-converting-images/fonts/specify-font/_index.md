---
title: Specify Font in EMF Images with Aspose.Imaging for .NET
linktitle: Specify Font
type: docs
weight: 30
url: /net/specify-font/
description: Demonstrates how to set a specific font when creating an EMF image.
keywords: font, emf, c#
---

# Specify Font in EMF Images with Aspose.Imaging for .NET

## Introduction
This example shows how to specify a custom font when generating an EMF (Enhanced Metafile) image using Aspose.Imaging for .NET. It is useful when you need precise control over the text rendering in vector graphics, such as mathematical symbols or brand‑specific typography.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Access to a TrueType font file (e.g., *Cambria Math*) placed in the working directory

## Step-by-step Guide
1. **Set the fonts folder** – Use `FontSettings.SetFontsFolder` to point Aspose.Imaging to the directory containing the desired font file.  
2. **Prepare Glyph indices** – Create an array of glyph indices that correspond to the symbols you want to render.  
3. **Create an EMF image** – Instantiate `EmfImage` with the required dimensions.  
4. **Add a font record** – Build an `EmfExtCreateFontIndirectW` object, configure its `EmfLogFont` (e.g., facename and height), and add it to the EMF records collection.  
5. **Add a text record** – Configure an `EmfExtTextOutW` object, set `ETO_GLYPH_INDEX` option, assign the glyph buffer, and add it to the records.  
6. **Select the font** – Insert an `EmfSelectObject` record to activate the previously defined font.  
7. **Save and render** – Call `emf.Save` to render the EMF content to an image format (e.g., PNG).  
8. **Clean up** – Optionally delete the temporary output file after verification.

## Code Example
The complete C# source for this scenario is shown below:

{{< gist "aspose-imaging-gists" "05d192da8185091b01d51f8892c0add7" "SpecifyFont.cs" >}}

## See Also
- **Working with Fonts in Aspose.Imaging** – Overview of font management capabilities.  
- **Creating EMF Images** – Basic guide to generating EMF graphics.  
- **Rendering Text with Glyph Indices** – Advanced technique for precise text rendering.
