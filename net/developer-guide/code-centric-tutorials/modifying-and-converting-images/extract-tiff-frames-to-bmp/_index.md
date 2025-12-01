---
title: Extract TIFF Frames to BMP Image Format
linktitle: Extract TIFF Frames to BMP
type: docs
weight: 30
url: /net/extract-tiff-frames-to-bmp/
description: Extract each frame from a multi-page TIFF file and save it as individual BMP images.
keywords: tiff bmp image conversion
---

# Extract TIFF Frames to BMP Image Format

## Introduction
This example demonstrates how to open a multi‑page TIFF image, iterate through its frames, and save each frame as a separate BMP file. Use it when you need to work with individual pages of a TIFF document in BMP format.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample multi‑page TIFF file (e.g., `SampleTiff1.tiff`) placed in the example's data directory

## Step-by-step Guide
1. Load the TIFF image using `Image.Load` and cast it to `TiffImage`.  
2. Loop through each `TiffFrame` in the image’s `Frames` collection.  
3. Set the current frame as the active frame.  
4. Extract the pixel data of the active frame with `LoadPixels`.  
5. Configure `BmpOptions` (e.g., 24 bits per pixel) and specify an output file path via `FileCreateSource`.  
6. Create a new `BmpImage` using `Image.Create` with the configured options and the frame’s dimensions.  
7. Write the extracted pixels to the BMP image with `SavePixels` and persist the file using `Save`.  
8. Increment a counter to generate unique output filenames for each frame.

## Code Example
The following gist contains the complete C# implementation of the example:

{{< gist "aspose-imaging-gists" "ec8e0d50cbe23bbd77e44682c87e353c" "ExtractTIFFFramesToBMPImageFormat.cs" >}}

## See Also
- Converting TIFF to PNG format
- Extracting pages from multi‑page PDF to images
- Changing image pixel format with Aspose.Imaging
