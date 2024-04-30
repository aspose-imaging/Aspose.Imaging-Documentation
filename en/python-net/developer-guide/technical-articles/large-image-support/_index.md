---
title: Large Image Support
type: docs
weight: 50
url: /python-net/large-image-support/
---

## **Large Image Support**
Since the standard libraries have some limitations as to the image size it can process, we introduced a new mechanism for large images support. The new approach overcomes the limitations but due to data size limitations the max supported dimensions for creation and loading are 2,147,483,647 x 2,147,483,647 pixels.

### **Working with Large Images**
Starting from Aspose.Imaging 1.8, we have totally reworked the architecture to improve Aspose.Imaging performance and support for large images. Images that are hundreds of megabytes in size is no longer a problem so you can create, load and draw over those images. However, due to the partial processing and handling of OutOfMemoryException exceptions, performance may be very low on very large images. This is due to the fact that Aspose.Imaging tries to re-allocate a smaller amount of data for processing and each reallocation step is very costly. The benefits of the new architecture are obvious: 

- There's no limitation to the image size.
- You are not limited to the memory available on your PC.

### **Supported Image Formats**
The following formats are supported for large images processing:

- BMP
- GIF
- TIFF
- PSD

The above formats may be safely processed through creation, loading, applying drawing operations, saving to disk or exporting between each other regardless of size. The JPG and PNG file formats do not support the large image architecture. If you try to export a BMP, GIF, TIFF or PSD image into other formats of images, you may get a OutOfMemoryException and processing will fail. There is no way to support large images for those formats. Aspose.Imaging will support large JPG and PNG images in the near future but until that you have to rely on smaller dimensions or on formats that support large dimensions.
