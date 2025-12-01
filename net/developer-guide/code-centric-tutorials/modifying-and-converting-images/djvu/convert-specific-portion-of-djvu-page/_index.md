---
title: Convert Specific Portion of DjVu Page
linktitle: Convert Specific Portion of DjVu Page
type: docs
weight: 30
url: /net/convert-specific-portion-of-djvu-page/
description: Extract and save a specific region from a DjVu page as a new DjVu file.
keywords: djvu conversion c#
---

# Convert Specific Portion of DjVu Page

## Introduction
This example demonstrates how to load a DjVu document, select a rectangular area on a specific page, and save that portion as a new DjVu file. Use it when you need to extract only part of a DjVu page rather than the whole image.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A DjVu source file (e.g., `Sample.djvu`) placed in the data directory

## Step-by-step Guide
1. **Load the DjVu image** – Use `Image.Load` to open the source DjVu file.
2. **Configure export options** – Create a `PngOptions` instance, set its `ColorType` to grayscale, and define a `Rectangle` that represents the area to extract.
3. **Specify the page and region** – Set `DjvuMultiPageOptions` with the target page index and the rectangle.
4. **Save the extracted region** – Call `image.Save` with the configured options to generate a new DjVu file containing only the selected portion.

## Code Example
The following code snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "d336942b89f55363fc90c72eab9a22d0" "ConvertSpecificPortionOfDjVuPage.cs" >}}

## See Also
- [Convert DjVu Page to PNG](/net/convert-djvu-page-to-png/)
- [Export DjVu Multi‑Page Document](/net/export-djvu-multipage/)
- [Working with DjVu Images](/net/djvu-image-manipulation/)
