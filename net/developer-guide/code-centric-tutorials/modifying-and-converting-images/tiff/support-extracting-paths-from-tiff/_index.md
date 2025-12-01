---
title: Extract Paths from TIFF Images with Aspose.Imaging for .NET
linktitle: Extract TIFF Paths
type: docs
weight: 30
url: /net/support-extracting-paths-from-tiff/
description: Demonstrates how to read and create path resources in a TIFF image using Aspose.Imaging for .NET.
keywords: tiff path extraction c#
---

# Extract Paths from TIFF Images

## Introduction
This example shows how to enumerate existing path resources in a TIFF file and how to create a new clipping path programmatically. Use it when you need to work with vector paths embedded in TIFF images, such as for Photoshop‑compatible editing or exporting.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample TIFF file named **Sample.tif** placed in the data directory used by the examples

## Step-by-step Guide
1. Load the TIFF image using `Image.Load` and cast it to `TiffImage`.
2. Iterate through `image.ActiveFrame.PathResources` to read the names of existing paths.
3. Save the image to another format (e.g., PSD) to verify extracted paths.
4. Create a new `PathResource` with a custom name and a collection of `VectorPathRecord` objects.
5. Assign the new list to `image.ActiveFrame.PathResources` and save the modified image back to TIFF.
6. Clean up any intermediate files created during the process.

## Code Example
The following code demonstrates extracting existing paths and adding a new clipping path to a TIFF image:

{{< gist "aspose-imaging-gists" "140bbbd3c9a491887f1ed8d16d82fe85" "SupportExtractingPathsFromTiff.cs" >}}

## See Also
- **Working with Vector Paths in TIFF** – deeper dive into path records and Photoshop specifications.  
- **Converting TIFF to Other Formats** – how to convert TIFF images to PNG, JPEG, or PSD using Aspose.Imaging.  
- **Saving Images with Different Options** – overview of image saving options and format‑specific settings.
