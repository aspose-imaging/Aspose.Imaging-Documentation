---
title: Working with multipage image formats
type: docs
weight: 90
url: /ru/net/working-with-multipage-image-formats/
---

Aspose.Imaging supports rich functionality to work with multipage image formats such as Gif, Tiff, Psd, Dicom, Cdr, WebP etc. Also, using Aspose.Imaging image can be exported also to multipage PDF document.

To indicate whether the image contains layers/pages/ frames the *IMultipageImage interface* has been introduced. All multi-page images such as PSD, CDR, GIF, etc. are descendants of this interface. Using Pages property, you can access the pages of any multi-page image in the library.

**Example of usage IMultipageImage interface:**

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "imultipage-image.cs" >}}


**Export of multipage images** can be performed using MultiPageOptions class. With this option you can specify the pages that you want to export to another format. In the case of export to a single-page format, the 1st page of the range will be exported; in the case of export to a multi-page format, all pages of the range will be exported.

**Example of export from multi-page format to single-page image format:**

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "export-multipage-images.cs" >}}

**Example of export from multi-page format to multi-page**

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "export-from-multipage-to-multipage.cs" >}}

Here the 4th and 5th pages will be exported to the tiff format

Below presented **example of export from/to different multipage image formats**:

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "export-from-to-different-multipage-formats.cs" >}}

## **Support of making gifs and other multi-page (multi-frame) files from set of images**

### **Create multipage images using AddPage method**

You can create multipage image using AddPage() method. The following code shows how you can **create animated images using image frames from the folder**:

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "create-multipage-images-using-add-page.cs" >}}

### **Create multipage image from vector images**

In order to use vector images as animation frames you need to rasterize them first. The following source code sample shows how to **create TIFF image using vector images**:

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "create-multipage-image-from-vector-images.cs" >}}

### **Create animation from an array of images**

{{< gist "aspose-com-gists" "af09b6dfc586ad81f2bc7806eff52a20" "create-animation-from-array-of-images.cs" >}}

