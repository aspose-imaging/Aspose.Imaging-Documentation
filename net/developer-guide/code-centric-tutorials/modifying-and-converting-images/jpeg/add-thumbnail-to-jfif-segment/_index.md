---
title: Add Thumbnail to JFIF Segment in JPEG Image
linktitle: Add Thumbnail to JFIF Segment
type: docs
weight: 30
url: /net/add-thumbnail-to-jfif-segment/
description: Demonstrates how to embed a thumbnail into the JFIF segment of a JPEG image using Aspose.Imaging for .NET.
keywords: jpeg, thumbnail, c#
---

# Add Thumbnail to JFIF Segment in JPEG Image

## Introduction
This example shows how to create a thumbnail image and embed it into the JFIF (JPEG File Interchange Format) segment of a JPEG file. Use it when you need to add or replace thumbnails inside JPEG images without altering the main picture data.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library installed via NuGet
- Access to a writeable folder for saving the output JPEG file

## Step-by-step Guide
1. **Prepare the working directory** – Obtain the path to the folder that contains sample JPEG files.
2. **Create a thumbnail image** – Instantiate a `JpegImage` object with the desired thumbnail dimensions (e.g., 100 × 100 pixels).
3. **Create the target JPEG image** – Instantiate another `JpegImage` object representing the image that will hold the thumbnail.
4. **Assign the thumbnail to the JFIF segment** – Set the `Jfif.Thumbnail` property of the main image to the thumbnail image created in step 2.
5. **Save the modified image** – Call `Save` on the main image, specifying an output file name (e.g., `AddThumbnailToJFIFSegment_out.jpeg`).

## Code Example
Below is the complete code snippet for this workflow.

{{< gist "aspose-imaging-gists" "75e07b774d0843c7e6671006c26e987c" "AddThumbnailToJFIFSegment.cs" >}}

## See Also
- Adding custom metadata to JPEG images
- Converting JPEG images to other formats with Aspose.Imaging
- Resizing and cropping images using Aspose.Imaging for .NET
