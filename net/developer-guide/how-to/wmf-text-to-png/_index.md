---
type: docs
weight: '90'
url: /net/developer-guide/how-to/wmf-text-to-png
title: Textual Wmf to Png conversion
---

**Support textual Wmf to Png conversion**
-----------------------------------------

**Issue** : When converting WMF file to PNG, the text position and style can change.

**Tips** : It is necessary to change the RenderMode property to Auto in
WmfRasterizationOptions.

**Example :**

{{< gist "aspose-com-gists" "f000a778d6a34a61caa392e1804d1ff8" "wmf-text-to-png.cs" >}}
