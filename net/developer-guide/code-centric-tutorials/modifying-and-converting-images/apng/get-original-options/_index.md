---
title: Retrieve Original APNG Options with Aspose.Imaging
linktitle: Get Original Options
type: docs
weight: 30
url: /net/get-original-options/
description: Shows how to obtain the original APNG image options using Aspose.Imaging for .NET.
keywords: apng options c#
---

# Retrieve Original APNG Options

## Introduction
This example demonstrates how to extract the original image options from an APNG file using Aspose.Imaging for .NET. It is useful when you need to inspect or verify the default settings (such as number of plays, frame time, and bit depth) of an APNG image before performing further processing.

## Prerequisites
- .NET 5.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- An APNG image file (e.g., **SteamEngine.png**) placed in the example data folder

## Step-by-step Guide
1. **Prepare the data directory** – Locate the folder that contains the sample APNG file.
2. **Load the APNG image** – Use `Image.Load` to read the file into an `ApngImage` instance.
3. **Retrieve the original options** – Call `image.GetOriginalOptions()` and cast the result to `ApngOptions`.
4. **Validate the options** – Check properties such as `NumPlays`, `DefaultFrameTime`, and `BitDepth` to ensure they match expected defaults.
5. **Dispose resources** – The `using` statement automatically releases the image resources.

## Code Example
The following code snippet contains the complete implementation of the steps described above:

{{< gist "aspose-imaging-gists" "d11ab7adc16aa94bcd41dd5af1ac1021" "GetOriginalOptions.cs" >}}

## See Also
- Loading an APNG image with Aspose.Imaging
- Modifying APNG frame timing and playback options
- Converting APNG to other image formats (e.g., PNG, GIF)
