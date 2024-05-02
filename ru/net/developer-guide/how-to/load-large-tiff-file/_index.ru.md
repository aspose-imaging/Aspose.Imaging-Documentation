---
type: docs
weight: '90'
url: /ru/net/developer-guide/how-to/load-large-tiff-file
title: How to load large tiff file when memory not enought
linktitle: How to load large tiff file when memory not enought
description: Sometimes it is needed to load large tiff file but memory is not enought to process it.
---

**How to load large tiff file when there is not enought memory**
-----------------------------------------

**Issue** : Fails to load large tiff file.

**Tips** : To load large tiff images there can be used memory strategy optimization be specifying buffersizehint property for your PC.

**Example :**

{{< gist "aspose-com-gists" "3fd62316b7516c54cdec5700f6785166" "memory-strategy-optimization-tiff.cs" >}}
