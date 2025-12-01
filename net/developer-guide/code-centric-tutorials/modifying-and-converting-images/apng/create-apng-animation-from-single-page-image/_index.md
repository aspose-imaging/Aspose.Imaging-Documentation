---
title: Create APNG Animation from a Single‑Page Image
linktitle: Create APNG Animation
type: docs
weight: 30
url: /net/create-apng-animation-from-single-page-image/
description: Creates an animated APNG by adding frames to a single‑page PNG image.
keywords: apng animation c#
---

# Create APNG Animation from a Single‑Page Image

## Introduction
This example shows how to generate an animated APNG (Animated Portable Network Graphics) file by repeatedly adding frames to a single‑page PNG image. It demonstrates frame‑by‑frame manipulation, gamma adjustment, and saving the final animated image.

## Prerequisites
- .NET 9.0 (or later)
- Aspose.Imaging for .NET library
- A non‑animated PNG source file (e.g., `not_animated.png`) placed in the data directory used by the examples

## Step-by-step Guide
1. Load the source PNG image using `Image.Load`.
2. Create an `ApngOptions` object, specifying the output file path, default frame time, and color type.
3. Initialise an `ApngImage` with the desired dimensions via `Image.Create`.
4. Remove any existing frames from the `ApngImage`.
5. Add the first frame using `apngImage.AddFrame`.
6. Loop to add intermediate frames, adjusting each frame’s gamma with `ApngFrame.AdjustGamma`.
7. Add the final frame.
8. Save the animated APNG using `apngImage.Save`.
9. (Optional) Delete the generated file after verification.

## Code Example
The following code demonstrates how to create the APNG animation:

{{< gist "aspose-imaging-gists" "ee2276709661dc43611b1314c2b212cc" "CreateAPNGAnimationFromSinglePageImage.cs" >}}

## See Also
- Converting PNG to APNG
- Modifying frames of an existing APNG
- Creating animated GIFs with Aspose.Imaging for .NET
