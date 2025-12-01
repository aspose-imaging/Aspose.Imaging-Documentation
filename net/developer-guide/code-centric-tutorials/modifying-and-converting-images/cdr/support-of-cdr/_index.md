---
title: Support of CDR Files
linktitle: Support of CDR
type: docs
weight: 30
url: /net/support-of-cdr/
description: Demonstrates how to verify that Aspose.Imaging for .NET supports CorelDRAW (CDR) files.
keywords: cdr aspnet support
---

# Support of CDR Files

## Introduction
This example shows how to confirm that Aspose.Imaging for .NET can recognize and work with CorelDRAW (CDR) files. It is useful when you need to validate file‑format support before performing any image operations.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- A sample CDR file (e.g., `test.cdr`) placed in the example data folder

## Step-by-step Guide
1. Determine the data directory that contains the sample CDR file.  
2. Define the expected file format using `FileFormat.Cdr`.  
3. Load the image with `Image.Load`.  
4. Compare the loaded image’s `FileFormat` with the expected format.  
5. Throw an exception if the formats do not match; otherwise, proceed knowing the CDR format is supported.

## Code Example
The following example demonstrates how to check CDR support:

{{< gist "aspose-imaging-gists" "6552eb1def0bbeb2302e3817026d2c37" "SupportOfCDR.cs" >}}

## See Also
- Loading CDR Images  
- Converting CDR to Other Formats  
- Working with Vector Images in Aspose.Imaging
