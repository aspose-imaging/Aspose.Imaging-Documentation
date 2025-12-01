---
title: Save EMF+ Image to File using Aspose.Imaging
linktitle: Save EMF+ to File
type: docs
weight: 30
url: /net/save-emfplus-to-file/
description: Demonstrates how to load an EMF+ meta image and save it as a separate EMF file with Aspose.Imaging for .NET.
keywords: emfplus c# save
---

# Save EMF+ Image to File

## Introduction
This example shows how to load an EMF+ (Enhanced Metafile) image, manipulate it as a `MetaImage`, and then save it as a standard EMF file. It is useful when you need to convert or extract vector graphics stored in EMF+ format.

## Prerequisites
- .NET 6.0 or later
- Aspose.Imaging for .NET library
- An EMF+ file named `TestEmfPlusFigures.emf` placed in the example data folder

## Step-by-step Guide
1. **Locate the data directory** – Retrieve the path where the example EMF+ file is stored.  
2. **Load the EMF+ image** – Use `Image.Load` to open the file as a `MetaImage`.  
3. **Save the image** – Call `image.Save` with the desired output path and an `EmfOptions` instance to produce a standard EMF file.  
4. **Verify the result** – The new file will have the same name with an additional `.emf` extension.

## Code Example
The following snippet demonstrates the complete process:

{{< gist "aspose-imaging-gists" "8109bb799f787cba3dde4c105ce609b6" "SaveEMFPlustoFile.cs" >}}

## See Also
- Converting EMF to PNG with Aspose.Imaging
- Modifying EMF metadata programmatically
- Working with vector images in Aspose.Imaging for .NET
