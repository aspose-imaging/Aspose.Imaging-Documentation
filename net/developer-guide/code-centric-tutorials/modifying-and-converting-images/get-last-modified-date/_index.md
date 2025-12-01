---
title: Get Last Modified Date of an Image
linktitle: Get Last Modified Date
type: docs
weight: 20
url: /net/get-last-modified-date/
description: Shows how to retrieve the last modified date of an image using Aspose.Imaging for .NET.
keywords: last modified date, image metadata, c#
---

# Get Last Modified Date of an Image

## Introduction
This example demonstrates how to obtain the last modified date of an image file using Aspose.Imaging for .NET. It shows two approaches: retrieving the date from the file system and from XMP metadata when available. Use this when you need to audit or display image modification timestamps.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- A sample image file (e.g., `aspose-logo.jpg`) placed in the project’s data directory

## Step-by-step Guide
1. **Prepare the data directory** – Locate the folder containing the sample image.
2. **Load the image** – Use `Image.Load` to create a `RasterImage` instance from the file.
3. **Retrieve modify date from file system** – Call `image.GetModifyDate(true)` to get the `FileInfo`‑based date.
4. **Retrieve modify date from XMP metadata** – Call `image.GetModifyDate(false)`; this falls back to the file system date if XMP metadata is missing.
5. **Display the results** – Output the obtained dates to the console or logger.
6. **Dispose the image** – Ensure the `RasterImage` object is properly disposed (e.g., via a `using` statement).

## Code Example
The following code snippet illustrates the complete workflow:

{{< gist "aspose-imaging-gists" "945f465c84ba0d8d514a22997373d261" "GetLastModifiedDate.cs" >}}

## See Also
- Reading image metadata with Aspose.Imaging
- Accessing EXIF properties of an image
- Saving an image in a different format using Aspose.Imaging
