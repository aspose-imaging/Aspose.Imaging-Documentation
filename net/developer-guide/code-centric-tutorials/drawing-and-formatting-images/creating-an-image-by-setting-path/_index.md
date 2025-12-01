---
title: Create an Image by Setting a File Path
linktitle: Create Image by Path
type: docs
weight: 30
url: /net/creating-an-image-by-setting-path/
description: Demonstrates how to generate a BMP image by specifying a file path using Aspose.Imaging for .NET.
keywords: create image c#
---

# Create an Image by Setting a File Path

## Introduction
This example illustrates how to programmatically create a BMP image by defining the output file path with **BmpOptions** and **FileCreateSource**. Use it when you need to generate images on the fly and control where they are saved.

## Prerequisites
- .NET (any recent version, e.g., .NET 6 or later)
- Aspose.Imaging for .NET library
- Write permission to a folder where the image will be saved

## Step-by-step Guide
1. Retrieve the directory that holds example data files.  
2. Instantiate **BmpOptions** and set desired properties such as **BitsPerPixel**.  
3. Assign a **FileCreateSource** to the **Source** property of **BmpOptions**, providing the full path for the new image file.  
4. Call **Image.Create** with the configured options and the required width and height.  
5. Save the created image to the target location using **image.Save**.  
6. Dispose of the image object (handled automatically with a `using` block).

## Code Example
The following code demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "16072e5228acf9b4e3460c9980f793bd" "CreatingAnImageBySettingPath.cs" >}}

## See Also
- Loading and saving images with Aspose.Imaging
- Drawing shapes and text on images
- Converting images between different formats
