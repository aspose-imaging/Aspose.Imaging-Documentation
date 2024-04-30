---
title: Compressed vector formats
type: docs
weight: 10
url: /python-net/compressed-vector-formats/
---

Compressed vector images are vector images of the EMF, WMF, SVG formats compressed using a zip archiver. Their size averages from 30-70% of the original. This saves space on media and reduces file transfer time over the network. But you should pay attention to the fact that not all applications work with compressed vector formats. See below for more details.

## SVGZ
SVGZ files are typically 50 to 80 percent smaller in size than SVG.
For example, take any SVG file and compress it to SVGZ:

{{% image img="compressed-vector-formats_1.png" alt="Svg source file before the compression" %}}

As you can see the size of the source file is **369** kb

**Convert SVG to SVGZ** using the following code:

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-svg-to-svgz.py" >}}

{{% image img="compressed-vector-formats_2.png" alt="Svgz compression" %}}

The resulting file size is  ~**59%** of the original.
We can open this file using any of the above applications.

{{% image img="compressed-vector-formats_3.png" alt="Svgz compression result" %}}

Using the following code, it is possible to **convert the SVGZ to SVG:**

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-svgz-to-svg.py" >}}

## EMZ
A file with the EMZ file extension is a  actually just GZIP compressed EMF files, which is a graphics format used by Microsoft (**MS Word, MS Visio**)

For example, take any EMF file and compress it to EMZ:

{{% image img="compressed-vector-formats_4.png" alt="todo:image_alt_text" %}}

As you can see the size of the source file is **116** kb
**Convert EMF to EMZ** using the following code:

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-emf-to-emz.py" >}}

{{% image img="compressed-vector-formats_5.png" alt="todo:image_alt_text" %}}

The resulting file size is  ~**14%** of the original.

Open result emz file in MS Word

Using the following code, it is possible to **convert the EMZ to EMF**

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-emz-to-emf.py" >}}

## WMZ
A file with the WMZ file extension is a  actually just GZIP compressed WMF files, which is a graphics format used by Microsoft (**MS Word, MS Visio**).

For example, take any WMF file and compress it to WMZ:

{{% image img="compressed-vector-formats_6.png" alt="todo:image_alt_text" %}}

As you can see the size of the source file is **55.2** kb. **Convert WMF to WMZ** using the following code:

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-wmf-to-wmz.py" >}}

{{% image img="compressed-vector-formats_7.png" alt="todo:image_alt_text" %}}

The resulting file size is  ~**49%** of the original.

Open result emz file in MS Word

{{% image img="compressed-vector-formats_8.png" alt="todo:image_alt_text" %}}

Using the following code, it is possible to **convert the WMZ to WMF:**

{{< gist "aspose-com-gists" "62318d9a15ea68c4557201ad9f90396c" "convert-wmz-to-wmf.py" >}}
