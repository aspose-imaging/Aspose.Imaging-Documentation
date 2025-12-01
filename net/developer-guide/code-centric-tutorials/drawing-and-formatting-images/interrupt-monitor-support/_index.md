---
title: Using InterruptMonitor to Cancel Image Saving Operations
linktitle: Interrupt Monitor Support
type: docs
weight: 30
url: /net/interrupt-monitor-support/
description: Demonstrates how to interrupt an image conversion using InterruptMonitor in Aspose.Imaging for .NET.
keywords: interrupt monitor, image conversion, c#
---

# Using InterruptMonitor to Cancel Image Saving Operations

## Introduction
This example shows how to use **InterruptMonitor** to stop an ongoing image conversion process. It is useful when you need to enforce time‑outs or provide user‑controlled cancellation for long‑running image operations.

## Prerequisites
- .NET 9.0 (or later) runtime
- Aspose.Imaging for .NET library
- Sample image file (e.g., `aspose-logo_tn.jpg`) placed in the example data folder

## Step-by-step Guide
1. **Prepare the source and destination paths** – locate the input image and define where the output should be saved.  
2. **Create an `InterruptMonitor` instance** – this object will be used to signal an interruption.  
3. **Configure save options** – for this example a `PngOptions` object is used.  
4. **Instantiate a `SaveImageWorker`** – pass the input path, output path, save options, and the monitor to the worker class.  
5. **Run the worker on a separate thread** – start the thread that performs the image saving operation.  
6. **Allow the conversion to run briefly** – pause the main thread (e.g., 3 seconds) to let the save process begin.  
7. **Trigger the interruption** – call `monitor.Interrupt()` to request cancellation of the ongoing save.  
8. **Wait for the worker thread to finish** – `thread.Join()` ensures the main thread waits for completion.  
9. **Clean up** – delete the partially created output file if it exists.

## Code Example
The following code shows the complete example:

{{< gist "aspose-imaging-gists" "d50e8875ddb442c5758066f52681718e" "InterruptMonitorSupport.cs" >}}

## See Also
- Working with Multithreading in Aspose.Imaging
- Handling `OperationInterruptedException` in image processing
- Saving images in different formats with Aspose.Imaging
