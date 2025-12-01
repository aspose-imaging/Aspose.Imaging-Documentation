---
title: Track Image Loading and Export Progress Using Aspose.Imaging
linktitle: Document Conversion Progress
type: docs
weight: 30
url: /net/document-conversion-progress/
description: Demonstrates how to monitor load and export operations with progress event handlers.
keywords: progress events c#
---

# Track Image Loading and Export Progress

## Introduction
This example shows how to attach progress event handlers to image loading and exporting operations using Aspose.Imaging for .NET. It is useful when you need real‑time feedback on long‑running image processing tasks.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- Sample JPEG file (e.g., `aspose-logo.jpg`) placed in the example data directory

## Step-by-step Guide
1. Obtain the path to the sample image directory.  
2. Load the image with a `LoadOptions` object that specifies a `ProgressEventHandler`.  
3. Save the image using `JpegOptions`, providing another `ProgressEventHandler` for export progress.  
4. Implement the progress callbacks to write the current event type and progress values to the console.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "1e7db04ecd185aac96f3d3a32ae87804" "DocumentConvertionProgress.cs" >}}

## See Also
- [Loading and Saving Images with Aspose.Imaging](#)
- [Working with JPEG Options](#)
- [Handling Image Formats in Aspose.Imaging](#)
