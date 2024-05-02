---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/load-large-tiff-file
title: How to load large tiff file when memory not enough
linktitle: How to load large tiff file when memory not enough
description: Sometimes it is needed to load large tiff file but memory is not enough to process it.
---

**How to load large tiff file when there is not enough memory**
-----------------------------------------

**Issue** : Fails to load large tiff file.

**Tips** : To load large tiff images there can be used memory strategy optimization be specifying buffer_size_hint property for your PC.

**Example :**

{{< gist "aspose-com-gists" "fe159912bc60afbb34307153aa534ed3" "memory-strategy-optimization-tiff.py" >}}
