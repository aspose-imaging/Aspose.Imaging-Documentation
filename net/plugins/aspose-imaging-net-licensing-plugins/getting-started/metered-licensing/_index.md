---
title: Plugins Licensing - Metered License
type: docs
weight: 70
url: /net/plugins/aspose-imaging-net-licensing-plugins/metered-licensing/
description: Using the C# Image Processing Library licensing plugin to apply a metered key.
---

{{% alert color="primary" %}} 

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging licensing plugins introduce the capability for developers to apply a metered key, which represents a new licensing mechanism. The plugin licensing model imposes a restriction where only one plugin can be licensed within a single application instance. If entry points beyond the defined scope of the licensed plugin are utilized, the application automatically transitions to a trial operating mode. This ensures compliance with licensing terms while offering users the opportunity to explore additional functionalities through the trial mode. For further information, please consult the <a href="https://purchase.aspose.com/faqs/licensing/metered">Metered Licensing FAQ</a> section.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To obtain licenses, kindly visit the <a href="https://purchase.aspose.org/imaging">Aspose Purchase portal</a>.
</p>

{{% /alert %}} 

## **Metered Plugin Licensing**

Below are the straightforward steps to utilize the Metered class:

1. Instantiate the `Metered` class.
2. Provide the public and private keys using the `setMeteredKey` method.
3. Perform the necessary processing tasks.
4. Invoke the `getConsumptionQuantity` method of the Metered class.
5. This will yield the quantity of API requests consumed up to that point.

Here's a sample code illustrating how to set the metered public and private keys:

```cs
// Valid plugin license use example
Metered license = new Metered();
// Only one metered plug-in license is supported
license.SetMeteredKey("<your public key>", "<your private key>");
```    

Please see more Plugin Licensing [Use examples in C#](/imaging/net/plugins/developer-guide/use-examples/).
