---
title: Save Each Frame of a Multipage TIFF to PNG
linktitle: Save Each Frame to PNG
type: docs
weight: 30
url: /net/saving-each-frame-in-other-raster-image-format/
description: Demonstrates how to extract each frame from a multipage TIFF and save it as a PNG file using Aspose.Imaging for .NET.
keywords: tiff png c#
---

# Save Each Frame of a Multipage TIFF to PNG

## Introduction
This example shows how to load a multipage TIFF image, iterate through its frames, and save each frame as an individual PNG file. Use this when you need to work with single-page images extracted from a multi-frame document.

## Prerequisites
- .NET 6.0 or later (compatible with your project)
- Aspose.Imaging for .NET library installed via NuGet
- A sample multipage TIFF file (e.g., `SampleTiff1.tiff`) placed in the data directory

## Step-by-step Guide
1. Determine the directory that contains the source TIFF file.  
2. Load the TIFF image using `Image.Load` and cast it to `TiffImage`.  
3. Loop through the `Frames` collection of the loaded TIFF image.  
4. For each frame, call `Save` with a new file name and `PngOptions` to write the frame as a PNG file.  
5. Increment a counter to generate unique output file names for each frame.

## Code Example
Below is the complete example code that performs the described operations:

{{< gist "aspose-imaging-gists" "44024625e62c66101de29b05eaeb7668" "SavingEachFrameInOtherRasterImageFormat.cs" >}}

## See Also
- **Converting Image Formats** – Learn how to convert images between different file formats using Aspose.Imaging.  
- **Working with Multipage Images** – Explore other operations you can perform on multipage documents such as PDF or TIFF.  
- **Saving Images with Specific Options** – Understand how to customize image saving parameters like compression, resolution, and color depth.
