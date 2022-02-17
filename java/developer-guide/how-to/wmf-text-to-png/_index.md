---
type: docs
weight: '90'
url: /java/developer-guide/how-to/wmf-text-to-png
title: Textual Wmf to Png conversion
---

**Support textual Wmf to Png conversion**
-----------------------------------------

**Issue** : When converting WMF file to PNG, the text position and style can change.

**Tips** : It is necessary to change the RenderMode property to Auto in WmfRasterizationOptions.

**Example :**

{{< gist "aspose-com-gists" "297d9b641b096caa0706ce08da014dae" "wmf-text-to-png.java" >}}
