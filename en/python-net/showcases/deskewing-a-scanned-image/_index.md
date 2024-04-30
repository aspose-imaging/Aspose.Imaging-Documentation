---
title: Deskewing a scanned image
type: docs
weight: 30
url: /python-net/deskewing-a-scanned-image/
---

Skew is an artifact that might appear during document scanning process and it consists of getting the document’s text/images be rotated at a slight angle. It can have various causes but the most common are paper getting misplaced during a scan. Therefore, **deskew** is the process of detecting and fixing this issue on scanned files (ie, bitmap) so deskewed images will have the text/images correctly and horizontally aligned.

Deskewing an image can help a lot, if you want to improve the readability of scanned images. For example, think of a camera that automatically takes photos of goods with a barcode. If the skew angle is too high, the barcode can not be detected. After deskewing, the barcode can be read.

{{< gist "aspose-com-gists" "10a4ae814eef7b22d48295a8fa9d0d1d" "deskew.py" >}}

Below is an example of skewed scanned text and deskewed output.

| {{< image img="deskewing-a-scanned-image_1.png" alt="Skewed image">}} | {{< image img="deskewing-a-scanned-image_2.png" alt="Deskewed image">}} |
| ------------------------------------------------------- | ------------------------------------------------------- |
| Skewed image                                            | Deskewed image                                          |
