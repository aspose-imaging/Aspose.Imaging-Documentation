---
title: Plugins Licensing for Java - Metered License
type: docs
weight: 70
url: /java/aspose-imaging-java-licensing-plugins/metered-licensing/
description: Apply a metered key using the Aspose.Imaging Java Image Processing Library licensing plugin.
---

{{% alert color="primary" %}} 

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Aspose.Imaging licensing plugins enable developers to implement a metered key, introducing a new licensing mechanism. This plugin model restricts licensing to one plugin per application instance, transitioning the application to trial mode if entry points beyond the licensed plugin's scope are utilized. This approach ensures adherence to licensing terms while allowing users to explore additional functionalities through trial mode. Refer to the <a href="https://purchase.aspose.com/faqs/licensing/metered">Metered Licensing FAQ</a> for more details.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To acquire licenses, please visit the <a href="https://purchase.aspose.org/imaging">Aspose Purchase portal</a>.
</p>

{{% /alert %}} 

## **Metered Plugin Licensing**

Below are the simple steps to make use of the Metered class:

1. Initialize an instance of the `Metered` class.
2. Supply the public and private keys using the `setMeteredKey()` method.
3. Carry out the required processing tasks.
4. Call the `getConsumptionQuantity()` method from the Metered class.
5. This method will furnish the quantity of API requests utilized up to that point.

```java
com.aspose.imaging.Metered metered = new com.aspose.imaging.Metered();

//Specify public and private metered keys
metered.setMeteredKey(publicKey, privateKey);

//getConsumptionQuantity of the Metered class.
BigDecimal credit = com.aspose.imaging.Metered.getConsumptionCredit();
BigDecimal quanity = com.aspose.imaging.Metered.getConsumptionQuantity();
```    

Please see additional examples for specific scenarios demonstrated with Plugin Licensing in Java: [Use examples in Java](/imaging/java/plugins/developer-guide/use-examples/). 
