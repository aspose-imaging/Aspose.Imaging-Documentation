---
title: Convert a Range of DjVu Pages to Separate Images
linktitle: DjVu Pages to Images
type: docs
weight: 30
url: /net/convert-range-of-djvu-pages-to-separate-images/
description: Extract multiple DjVu pages and save each as a separate BMP image.
keywords: djvu convert c#
---

# Convert a Range of DjVu Pages to Separate Images

## Introduction
This example demonstrates how to load a DjVu document, select a specific range of pages, and export each page as an individual BMP image. Use it when you need to process or display individual pages from a multi-page DjVu file.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A DjVu file named **Sample.djvu** placed in the example data folder

## Step-by-step Guide
1. **Initialize the data directory** – Locate the folder that contains the source DjVu file.  
2. **Load the DjVu image** – Use `Image.Load` to open the DjVu document.  
3. **Configure BMP export options** – Create a `BmpOptions` instance and set `BitsPerPixel` to 32 for high‑color output.  
4. **Define the page range** – Instantiate an `IntRange` with the start and end page indexes you wish to export.  
5. **Iterate through the range** – For each page index:
   - Set `MultiPageOptions` on the BMP options to target the current page.
   - Call `image.Save` with a unique file name (e.g., `0_out.bmp`, `1_out.bmp`, …) to write the page as a separate BMP file.  
6. **Dispose resources** – The `using` block ensures the DjVu image is released after processing.

## Code Example
The following snippet shows the complete implementation:

{{< gist "aspose-imaging-gists" "d2ce57c1316802b90dcd6eb244f94340" "ConvertRangeOfDjVuPagesToSeparateImages.cs" >}}

## See Also
- **Convert DjVu to PDF** – Learn how to convert an entire DjVu document to a single PDF file.  
- **Export DjVu Pages to PNG** – A similar example that saves pages as PNG images instead of BMP.  
- **Working with Multi‑Page Images** – Overview of Aspose.Imaging’s multi‑page image handling capabilities.
