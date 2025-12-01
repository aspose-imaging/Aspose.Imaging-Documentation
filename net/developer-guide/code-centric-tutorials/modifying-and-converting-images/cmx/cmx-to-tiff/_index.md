---
title: Convert CMX to TIFF Using Aspose.Imaging for .NET
linktitle: CMX to TIFF
type: docs
weight: 30
url: /net/cmx-to-tiff/
description: Demonstrates how to convert a CMX vector image to a multipage TIFF with Aspose.Imaging for .NET.
keywords: cmx tiff conversion c#
---

# Convert CMX to TIFF Using Aspose.Imaging for .NET

## Introduction
This example shows how to load a CMX vector image, rasterize each page, and export it as a multipage TIFF file. Use it when you need to convert legacy CMX documents to a widely supported TIFF format.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample CMX file (e.g., `MultiPage2.cmx`) placed in the example data folder

## Step-by-step Guide
1. **Locate the data directory** – Obtain the path where the sample CMX file resides using `RunExamples.GetDataDir_CMX()`.  
2. **Load the CMX image** – Call `Image.Load` and cast the result to `VectorMultipageImage`.  
3. **Create rasterization options** – Generate an array of `CmxRasterizationOptions`, one for each page, using helper methods that set the appropriate page size.  
4. **Configure TIFF export options** – Instantiate `TiffOptions` with the desired compression (`TiffDeflateRgb`) and assign the rasterization options via `MultiPageOptions`.  
5. **Save as TIFF** – Call `image.Save` with the target file name and the configured TIFF options.  
6. **Clean up** – Delete the generated TIFF file if needed.

## Code Example
The following snippet contains the complete example code:

{{< gist "aspose-imaging-gists" "0ded044fcba24d5a74656dfe3423c46c" "CmxToTiffExample.cs" >}}

## See Also
- Converting CMX to PNG with Aspose.Imaging
- Working with multipage TIFF files in Aspose.Imaging
- Rasterizing vector images to bitmap formats
