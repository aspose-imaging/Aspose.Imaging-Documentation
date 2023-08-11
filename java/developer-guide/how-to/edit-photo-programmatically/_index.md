---
type: docs
weight: '90'
url: /java/developer-guide/how-to/edit-photo-programmatically
linktitle: Edit photo or image programmatically
title: How to edit your photo or image programmatically
description: Library for image editing. Photo editing automation. Image manipulation by NET (Java) program. Removing photo background. Online photo editor.
keywords: [edit a photo, editing of pictures, edit an image, photo background editor, photo background change, resizing an image, resizing photos, photo sizing, picture resizer, image crop, crop photo, filter photo, online photo editor, online image editor, photo editing app, free photo editor]
---

## How to edit your photo or image programmatically

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Just as an eye-catching book cover often guarantees success among buyers, a well-crafted website is a guarantee of high attendance. Just as a potential reader wouldn't want to miss a publication after observing its cover on a store shelf, every element should be in harmony: the design, illustrations, well-chosen color palette, and appropriate fonts. The more attentive we are in selecting and processing images on a web page, the greater the likelihood that users will favor it. However, today's fast-paced lifestyle and intensifying competition set increasingly high benchmarks for material quality and efficiency. Equipped with a toolkit for image editing, you can enhance a website's appeal, leading to increased organic traffic.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Automating repetitive image editing tasks accelerates the process of preparing pictures for subsequent use, whether it's for a book illustration, a website, or a scientific research project. For instance, you can simultaneously apply filters like noise reduction or image smoothing to multiple files. The Aspose.Imaging software library for Java provides a comprehensive toolkit for image processing. Aspose.Imaging enables the creation of diverse web services, such as generating collages from multiple images or applying cartoonify effects to inspire pictures with an animated film style.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This article explains the practical use of highly efficient image editing tools provided by Aspose.Imaging Java library. Refer to the linked list of the <a href="https://docs.aspose.com/imaging/java/supported-file-formats/">supported image formats</a> to explore the full possibilities.
</p>

### Resizing an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Before publishing images on a website, it usually needs to prepare the initial images for various web presentation scenarios. For a photo gallery, thumbnails with smaller image dimensions are required, for photo previews, images need to be resized to medium sizes, and for detailed views, larger sizes are necessary. With the Aspose.Imaging library, executing an image resizing procedure for multiple files is straightforward, allowing you to generate a collection of images in the required sizes.
</p>

Java code example: [howto resize image](resize-image).


### Crop an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In certain situations, images may have key objects or specific figures in photos that you want to isolate and position in the central region of the image. You can define a rectangular area for this designated figure and achieve this image cropping using the methods provided by the Aspose.Imaging library.
</p>

Java code example: [howto crop image](crop-image).


### Rotate

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You might have a collection of images that you wish to rotate to a precise angle, either clockwise or counterclockwise. This could be necessary when a horizontal line within photos has an undesirable tilt. With the assistance of the Aspose.Imaging library, you can easily rotate images to any desired angle.
</p>

Java code example: [howto rotate image](rotate-image).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The more examples, how to resize, crop and rotate images you can find in the [Aspose.Imaging Developer's guide](https://docs.aspose.com/imaging/java/crop-rotate-and-resize-images/).


### Remove background

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Another common need for image editing tools is the background removal process. Users might want to eliminate a background entirely or replace it with a different color or even make it transparent. This task is straightforward when the figures are positioned against a uniform background, but it becomes challenging when dealing with intricate backgrounds containing various other objects. The Aspose.Imaging library offers a list of methods to handle complex scenarios. For simpler cases, you can rely on automatic techniques provided by Aspose.Imaging. However, for more complex situations, you might need to initiate a programmatic request using the Aspose Cloud API to identify objects within images and subsequently extract them from the background.
</p>

Original image:

<img src="images/original.webp" alt="Original image" width="639" height="424"/>

Image with automatically removed background:

<img src="images/remove-background_auto.webp" alt="Image with removed background" width="640" height="425"/>

Java code example: [howto remove background](remove-background).


### Filter an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Your photo will appear more captivating upon utilizing the Aspose.Imaging Java filters. These filters can be applied to entire images or specific rectangular areas. In the latter scenario, you'll realize an effect like to looking through a specialized glass placed in front of your photo. This glass either blurs or sharpens objects as observed through it.
</p>

Original image:

<img src="images/sample.webp" alt="Original image sample" width="640" height="360"/>

Image with Gauss blur filter:

<img src="images/gauss_blur_filter.webp" alt="image with Gauss blur filter" width="640" height="360"/>

Java code example: [howto filter image](filter-image).


### Merge images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging for Java enables you to seamlessly combine multiple images either horizontally or vertically. This capability can be employed for crafting collages or even for generating larger wallpapers through the repetition of a pattern using smaller images.
</p>

Merged two images info one collage:

<img src="images/merge_images.webp" alt="Merged two images info one collage" width="640" height="180"/>

Java code example: [howto merge images](merge-images).


### Grayscale image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Have you ever observed how the same image, when transformed into grayscale, appears distinct and often more captivating than its original color version? Grayscale transformation can sometimes convey more profound meaning. By removing color information, you're able to distinguish delicate details within the image, and the interplay of light and shadow assumes a more prominent role. Aspose.Imagine for Java provides a solution for generating grayscale versions of both raster and vector image formats using rasterize technics.
</p>

Grayscaled image example:

<img src="images/Grayscaling_out.webp" alt="Image converted to Grayscale" width="640" height="360"/>

Java code example: [howto grayscale image](grayscale-image).


### Binarize image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can transform a color image into black and white by replacing each pixel with one of two binary values based on its intensity. If the pixel intensity is greater or less than a predefined threshold, a new value is assigned. The Aspose library also offers alternative methods for applying binarization, allowing for smoother outcomes to be achieved.
</p>

Example of black and image with binarization threshold 100:

<img src="images/BinarizationWithFixedThreshold_out.webp" alt="Image with binarize fixed threshold filter" width="640" height="360"/>

Java code example: [howto binarize image](binarize-image).


### Dither image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Preparing images for web publication can be a challenge, often resulting in undesirable quality problems when reducing the color palette of the images. However, utilizing the dithering method from the Aspose.Imaging tools can enhance image quality during such editing. There are various dithering options available, with the `FloydSteinberg` method being one of them, known for providing smoother results.
</p>

Example of image with `FloydSteinberg` dither method applied:

<img src="images/DitherImage_out.webp" alt="Dithered image for better quality" width="640" height="360"/>

Java code example: [howto dither image](dither-image).


### Adjust image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A photo with excessively dark or light areas appears weak. Additionally, unwanted color dominance can diminish the overall image impression. Using the Aspose image library for Java to adjust image brightness, contrast, and gamma correction can significantly enhance the situation and attract more users to a website.
</p>

Java code example: [howto adjust image](adjust-image).


### Cartoonify image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Using Aspose.Imaging, you can seamlessly apply various image editing techniques to craft unique visual effects. For instance, you can transform a photo into a captivating cartoon-style image. This involves applying several filters, adjusting brightness, binarizing, color replacement, and applying a mask to the original photo. Below is an example of a Java code snippet and the resulting image, illustrating the implementation of the cartoonify filter.
</p>

Example of image with `Cartoonify` filter applied:

<img src="images\cartoonify.webp" alt="Cartoon style image after cartoonify filter" width="960" height="266"/>

Java code example: [howto cartoonify image](cartoonify-image).


### Drawing images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging provides you with the capability to draw a range of shapes such as Lines, Rectangles, Arcs, or Bezier curves. You can form a Path by connecting multiple sequential graphical elements, enabling you to create complex figures with diverse colors and styles. You can select a Pen object or allocate a Brush object for drawing, and easily configure drawing parameters.
</p>

Java code example: [howto drawing images](draw-image).


## How to edit your photo or image online

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Finally, if you want to try a demo you can edit your pictures online. In case you need to edit only one photo or image, or you need to quickly apply filters to improve your photo, you can use Aspose online photo editing app as a free photo editor. Unlike paid versions of graphic editors, you can edit your photos in a web browser on Aspose website for free. With an online image editor, it is possible to make all common operations with your images. Open <a href="https://products.aspose.app/imaging/image-editor">Online image editor</a> in your browser and upload your image file from a local PC by drag-and-drop or upload an image from your Google or DropBox account into an active image editor area in your browser window. In the online editor, you can crop the image by selecting an arbitrary rectangle area or by selecting an area with a predefined sides ratio. Also, you can resize an image to a specific width and height or just indicate the scaling in percentages with keeping or not aspect ratio. Rotating and flipping images are available as well. You can rotate an image on a specific angle fitting to the canvas or cut edges after rotation.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
There are dozen of filters available on the <a href="https://products.aspose.app/imaging/photo-filter">Online photo editor</a>, including adjusting Brightness and Contrast, Gamma corrections, Grayscale, Binarize, Blur, Sharpen and Cartoon filters. After editing the image and applying filters you can save and download the resulting image using 20 available different popular image formats like `pdf`, `jpeg`, `gif`, `png` or `bmp`. You can check Aspose.Imaging program library functionality and quality by trying these online image editors, and decide to order a license for the Aspose.Imaging local usage to create your applications and services.
</p>


## Conclusion

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Imaging program library helps you to edit images and photos and facilitates the development of graphic manipulating applications and services. The image library provides you ready to use program methods to process images in your own way. Free online photo and images editor with photo filter is available at your convenience where you can try the most popular image editing operations and save the results in many image formats.
</p>
