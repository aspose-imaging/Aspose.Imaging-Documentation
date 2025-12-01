---
title: Using Metered Licensing with Aspose.Imaging for .NET
linktitle: Metered Licensing
type: docs
weight: 30
url: /net/metered-licensing/
description: Demonstrates how to configure metered licensing and retrieve consumption quantities.
keywords: metered licensing c#
---

# Using Metered Licensing with Aspose.Imaging for .NET

## Introduction
This example shows how to activate Aspose.Imaging's metered licensing model, set the required public and private keys, and read the consumption amount before and after invoking the API. Use it when you need to monitor usage costs in a metered deployment.

## Prerequisites
- .NET 6.0 or later (the example targets .NET 9.0)
- Aspose.Imaging for .NET library
- No additional files are required; the code runs as a console application.

## Step-by-step Guide
1. Create an instance of `Aspose.Imaging.Metered`.
2. Call `SetMeteredKey` with your public and private metered keys.
3. Retrieve the current consumption amount using `Metered.GetConsumptionQuantity()` before any API calls.
4. Perform the desired imaging operations (omitted for brevity).
5. Retrieve the consumption amount again after the operations to see the usage delta.
6. Optionally display the values in the console or log them for reporting.

## Code Example
The following snippet contains the complete implementation of the metered licensing workflow.

{{< gist "aspose-imaging-gists" "d227122f0abe833cdf837bbe2b9ba467" "MeteredLicensing.cs" >}}

## See Also
- Applying a regular (non‑metered) license with Aspose.Imaging
- Checking license expiration status
- Monitoring API usage programmatically in Aspose.Imaging
