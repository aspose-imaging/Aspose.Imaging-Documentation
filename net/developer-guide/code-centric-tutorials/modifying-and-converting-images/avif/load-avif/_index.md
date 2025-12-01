---
title: Load an AVIF Image with Aspose.Imaging for .NET
linktitle: Load AVIF Image
type: docs
weight: 10
url: /net/load-avif/
description: Demonstrates how to load an AVIF image using Aspose.Imaging for .NET.
keywords: avif image c#
---

# Load an AVIF Image

## Introduction
This example shows how to load an AVIF image file using the Aspose.Imaging for .NET library. It is useful when you need to read AVIF files for further processing, conversion, or analysis in your .NET applications.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0 in the source repository)
- Aspose.Imaging for .NET installed
- An AVIF file named `example.avif` placed in the data directory returned by `RunExamples.GetDataDir_AVIF()`

## Step-by-step Guide
1. Obtain the path to the AVIF data directory using `RunExamples.GetDataDir_AVIF()`.
2. Call `Image.Load` with the full path to `example.avif` and cast the result to `AvifImage`.
3. Use the loaded `AvifImage` instance for any required operations (the sample simply loads and disposes it).
4. Release resources by wrapping the image object in a `using` statement.

## Code Example
The following code demonstrates how to load an AVIF image:

{{< gist "aspose-imaging-gists" "da4c3977ab8d124cb9c0b815a46149c9" "LoadAvif.cs" >}}

## See Also
- Converting AVIF images to other formats
- Modifying AVIF image metadata
- Working with other image formats such as JPEG and PNG
