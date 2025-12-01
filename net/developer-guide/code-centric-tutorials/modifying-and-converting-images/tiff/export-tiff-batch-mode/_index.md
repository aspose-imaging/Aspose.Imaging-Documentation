---
title: Export TIFF Images in Batch Mode
linktitle: Export TIFF Batch Mode
type: docs
weight: 30
url: /net/export-tiff-batch-mode/
description: Demonstrates how to export TIFF images using batch mode to rotate pages efficiently.
keywords: tiff batch c#
---

# Export TIFF Images in Batch Mode

## Introduction
This example shows how to use Aspose.Imaging for .NET to export a multi‑page TIFF image while applying a batch operation to each page. It is useful when you need to process large TIFF files without loading all pages into memory at once.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample multi‑page TIFF file (e.g., `10MB_Tif.tif`) placed in the example data folder

## Step-by-step Guide
1. Load the source TIFF image using `Image.Load`.
2. Assign a delegate to the `PageExportingAction` property of the `TiffImage` instance.  
   - Inside the delegate, perform the desired operation on each page (e.g., rotate the page by 90°).  
   - Call `GC.Collect()` to free memory after processing each page.
3. Save the modified image to a new TIFF file with `tiffImage.Save`.
4. Note that after the batch save, all pages are released. Reload the image if further processing is required.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "9ea760d380825c1e2a6ef2160d7ccb98" "ExportTiffBatchMode.cs" >}}

## See Also
- [Converting Multi‑Page TIFF to PDF](#)
- [Optimizing Memory Usage When Processing Large Images](#)
