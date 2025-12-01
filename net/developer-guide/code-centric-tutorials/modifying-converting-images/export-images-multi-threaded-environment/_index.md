---
title: Export Images in a Multi‑Threaded Environment
linktitle: Export Images (Multi‑Threaded)
type: docs
weight: 20
url: /net/export-images-multi-threaded-environment/
description: Demonstrates how to export images safely in a multi‑threaded .NET application using Aspose.Imaging.
keywords: multithreaded, export images, Aspose.Imaging
---

# Export Images in a Multi‑Threaded Environment

## Introduction
This example shows how to export an image to a file stream while handling resources correctly in a multi‑threaded .NET environment. It is useful when you need to process or generate images concurrently without running into file access conflicts.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample BMP image file (e.g., `sample.bmp`) placed in the example data directory

## Step-by-step Guide
1. Determine the data directory that contains the source image.
2. Create a file stream for the target image file.
3. Configure `BmpOptions` with the desired pixel format and assign the stream as the source.
4. (Optional) Perform any image processing within a `using` block.
5. Ensure the file stream and image resources are properly disposed.
6. Delete the temporary file in a `finally` block to guarantee cleanup even if an exception occurs.

## Code Example
The following code illustrates the complete example:

{{< gist "aspose-imaging-gists" "0725f5d99df5d754ffd527d64a1102fa" "ExportImagesInMultiThreadedEnvironment.cs" >}}

## See Also
- Working with BMP images in Aspose.Imaging
- Ensuring thread safety with Aspose.Imaging API
- Processing images using streams in .NET
