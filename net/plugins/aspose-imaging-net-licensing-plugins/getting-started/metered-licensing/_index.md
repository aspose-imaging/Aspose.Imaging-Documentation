---
title: Plugins Licensing - Metered License
type: docs
weight: 70
url: /net/plugins/aspose-imaging-net-licensing-plugins/metered-licensing/
description: Using the C# Image Processing Library licensing plugin to apply a metered key.
---

{{% alert color="primary" %}} 

Aspose.Imaging licensing plugins introduce the capability for developers to apply a metered key, which represents a new licensing mechanism. This new method will complement the existing licensing approach. Customers who prefer to be billed based on their usage of the API features can opt for metered licensing. For further information, please consult the [Metered Licensing FAQ](https://purchase.aspose.com/faqs/licensing/metered) section.

{{% /alert %}} 

## **Metered Licensing**

Below are the straightforward steps to utilize the Metered class:

1. Instantiate the `Metered` class.
2. Provide the public and private keys using the `setMeteredKey` method.
3. Perform the necessary processing tasks.
4. Invoke the `getConsumptionQuantity` method of the Metered class.
5. This will yield the quantity of API requests consumed up to that point.

Here's a sample code illustrating how to set the metered public and private keys:

```cs
// Valid Animation plugin license use example
Metered license = new Metered();
// Only  metered plug-in license is supported
license.SetMeteredKey("<your public key>", "<your private key>");
```    

Please see more Plugin Licensing [Use C# examples](/imaging/net/plugins/developer-guide/use-examples/).
