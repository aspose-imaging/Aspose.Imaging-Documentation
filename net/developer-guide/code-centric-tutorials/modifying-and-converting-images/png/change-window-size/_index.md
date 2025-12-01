---
title: Change Window Size in PNG Images
linktitle: Change Window Size
type: docs
weight: 30
url: /net/change-window-size/
description: Demonstrates how to change the window size of a PNG image using Aspose.Imaging for .NET.
keywords: png resize .net
---

# Change Window Size in PNG Images

## Introduction
This example shows how to modify the window size of a PNG image by applying a binarization filter. Use it when you need to adjust image processing parameters for better visual results or downstream analysis.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A source PNG file (e.g., `test.png`) placed in the data folder

## Step-by-step Guide
1. **Set up the data directory** – Determine the folder that contains the source PNG file.  
2. **Load the PNG image** – Use `Image.Load` to read the file into a `PngImage` object.  
3. **Apply the window size change** – Call `image.BinarizeBradley` with the desired window width and height values.  
4. **Save the result** – Write the modified image to a new file (e.g., `result.png`).  
5. **Dispose resources** – The `using` statement automatically releases the image resources.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "6668f7ee2e3333ce33f18843f6ef11e3" "ChangeWindowSize.cs" >}}

## See Also
- Resizing Images in C# with Aspose.Imaging  
- Applying Binarization Filters to PNG Images  
- Modifying PNG Image Properties
