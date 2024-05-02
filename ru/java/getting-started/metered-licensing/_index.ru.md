---
title: Metered Licensing
type: docs
weight: 70
url: /ru/java/metered-licensing/
description: Developers can use the Java Image Processing Library API to apply a metered key, which is a new licencing mechanism.
---

{{% alert color="primary" %}} 

Aspose.Imaging allows developers to apply metered key. It is a new licensing mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. For more details, please refer to [Metered Licensing FAQ](https://purchase.aspose.com/faqs/licensing/metered) section.

{{% /alert %}} 
## **Metered Licensing**
Here are the simple steps to use the Metered class.

1. Create an instance of Metered class.
1. Pass public & private keys to setMeteredKey method.
1. Do processing (perform task).
1. call method getConsumptionQuantity of the Metered class.
1. It will return the amount/quantity of API requests that you have consumed so far.

Following is the sample code demonstrating how to set metered public and private key.

{{< gist "aspose-com-gists" "9656a0a7eedb4b07ab8a2922e161f63d" "apply-metered-license.java" >}}
