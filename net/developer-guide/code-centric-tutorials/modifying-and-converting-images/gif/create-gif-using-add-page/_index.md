---
title: Create a GIF Using AddPage Method
linktitle: Create GIF (AddPage)
type: docs
weight: 30
url: /net/create-gif-using-add-page/
description: Demonstrates how to create a multi‑page GIF by loading frames and adding them with AddPage.
keywords: gif addpage c#
---

# Create a GIF Using AddPage Method

## Introduction
- This example shows how to create a multi‑page GIF by loading individual PNG frames and adding them to a GIF image using the **AddPage** method.  
- Use it when you need to programmatically generate animated GIFs from separate image files.

## Prerequisites
- .NET 6.0 or later (the sample targets .NET 9.0)
- Aspose.Imaging for .NET library
- A folder containing PNG frames (e.g., an “Animation frames” directory)

## Step-by-step Guide
1. **Identify the source folder** that holds the PNG frames you want to animate.  
2. **Load each frame** into a `RasterImage` collection using `Image.Load`.  
3. **Create a `GifImage`** instance with the first frame supplied as the initial page.  
4. **Iterate over the remaining frames**, calling `image.AddPage(frame)` for each one.  
5. **Save the GIF** to the desired output location with `image.Save`.  
6. *(Optional)* Delete the generated GIF after verification to keep the workspace clean.

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "dde5dd23d7d15cb456f81993b84859bb" "CreateGifUsingAddPage.cs" >}}

## See Also
- Creating a GIF from a single image  
- Converting images to other formats (PNG, JPEG, TIFF, etc.)  
- Working with multi‑page TIFF files
