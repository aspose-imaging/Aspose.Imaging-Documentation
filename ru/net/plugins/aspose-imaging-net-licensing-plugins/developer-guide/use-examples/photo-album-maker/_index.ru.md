---
title: Photo Album Maker Licensing Plugin
type: docs
weight: 20
url: /ru/net/aspose-imaging-net-licensing-plugins/photo-album-maker/
description: Create photo albums in C# with the Photo Album Maker Plugin, seamlessly combining images and photos into multi-page albums, enabling the creation of multi-page files in various formats such as PDF and TIFF.
keywords: create photo album in C#, Photo Album Maker Plugin, combine images and photos, multi-page albums, create multi-page file, create PDF with images, create muti-page TIFF
---

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Photo Album Maker Licensing Plugin offers a convenient way to combine your images or photos into handy multi-page albums. You can utilize a variety of image files in different formats from the <a href="/imaging/ru/net/supported-file-formats/">list of supported image formats</a> to seamlessly merge them and create a single multi-page file such as a PDF or TIFF format. Before creating a photo album, ensure you acquire a Metered license by providing your public key and private password using the `SetMeteredKey()` method. In the C# code example below, we create a new `TiffImage` object and add existing images using the <a href="https://reference.aspose.com/imaging/ru/net/aspose.imaging.fileformats.tiff/tiffimage/addframe/">AddFrame()</a> method. If you prefer to create a PDF file containing your original images on separate pages, you can easily utilize the <a href="https://reference.aspose.com/imaging/ru/net/aspose.imaging/image/create/">Image.Create()</a> constructor with an array of images passed as a parameter and save the output to the file with `PdfOptions`. Please be aware that utilizing unlicensed features of the Aspose.Imaging graphic library will result in a watermark appearing on the output image.
</p>

{{< gist "aspose-com-gists" "01fededbe3304aa5de8d832a2a818ed0" "image-album-plugin-example.cs" >}}

Explore the functionalities of our free online <a href="https://products.aspose.app/imaging/photo-book-maker">Aspose.Imaging Photo Book Maker App</a> website.
