---
title: Using SyncRoot Property for Thread‑Safe Stream Access
linktitle: SyncRoot Property
type: docs
weight: 30
url: /net/sync-root-property/
description: Demonstrates how to use the SyncRoot property to synchronize access to a memory stream with Aspose.Imaging for .NET.
keywords: syncroot, thread safety, c#
---

# Use SyncRoot Property to Synchronize Stream Access

## Introduction
This example shows how to obtain a synchronization object (`SyncRoot`) from a `StreamContainer` and lock it while working with a memory stream. Use it when you need thread‑safe access to a stream that is shared across multiple threads.

## Prerequisites
- .NET 6.0 or later (compatible with Aspose.Imaging for .NET)
- Aspose.Imaging for .NET library installed
- No additional files are required; the example works entirely with an in‑memory stream

## Step-by-step Guide
1. Create a `MemoryStream` instance to hold image data in memory.  
2. Wrap the memory stream with `StreamContainer`, which provides the `SyncRoot` property.  
3. Use a `lock` statement on `streamContainer.SyncRoot` to ensure exclusive access while performing operations on the stream.  
4. Release the lock automatically when the `using` block ends.

## Code Example
The following snippet demonstrates the complete workflow:

{{< gist "aspose-imaging-gists" "73e5438d32fc70cc636540f0ba50fb60" "SyncRootProperty.cs" >}}

## See Also
- [Working with Memory Streams in Aspose.Imaging](#)
- [Thread‑Safe Image Processing with Aspose.Imaging](#)
- [Understanding StreamContainer and Its Properties](#)
