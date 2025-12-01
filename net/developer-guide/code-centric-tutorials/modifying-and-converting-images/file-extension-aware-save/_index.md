---
title: Save an Image with Automatic File Extension Detection
linktitle: File Extension Aware Save
type: docs
weight: 30
url: /net/file-extension-aware-save/
description: Demonstrates how to load an image and save it while automatically handling the file extension.
keywords: save image c#
---

# Save an Image with Automatic File Extension Detection

## Introduction
This example shows how to load an existing image and save it without explicitly specifying the output format. Aspose.Imaging automatically infers the correct format from the file extension of the target path. Use this approach when you want your code to adapt to different output extensions without extra conversion logic.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A sample image file (e.g., `aspose-logo.jpg`) placed in the example data folder

## Step-by-step Guide
1. Determine the folder that contains the source images (`dataDir`).
2. Build the full path for the output file, including the desired extension (e.g., `output.png`).
3. Load the source image using `Image.Load`.
4. Call `image.Save(outputPath)` – Aspose.Imaging detects the format from the `.png` extension.
5. (Optional) Delete the temporary output file if it was created only for demonstration purposes.

## Code Example
The following snippet contains the complete implementation of the example.

{{< gist "aspose-imaging-gists" "63a39d1a7ab1cf1d40bfb5520bbf7343" "FileExtensionAwareSave.cs" >}}

## See Also
- [Loading and Saving Images](/net/loading-and-saving-images/)
- [Converting Image Formats](/net/converting-image-formats/)
- [Modifying Image Properties](/net/modifying-image-properties/)
