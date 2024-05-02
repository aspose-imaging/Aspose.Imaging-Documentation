---
type: docs
weight: '90'
url: /ru/python-net/developer-guide/how-to/wmf-text-to-png
title: Textual Wmf to Png conversion in Python
linktitle: Textual Wmf to Png conversion
description: The text position and style can change while converting a WMF file to a PNG file, which can be managed using the Python Image Processing Library.
---

**Support textual Wmf to Png conversion**
-----------------------------------------

**Issue** : When converting WMF file to PNG, the text position and style can change.

**Tips** : It is necessary to change the RenderMode property to AUTO in
WmfRasterizationOptions.

**Example :**

{{< gist "aspose-com-gists" "9594d83600c932a0a865655c5e665add" "wmf-text-to-png.py" >}}
