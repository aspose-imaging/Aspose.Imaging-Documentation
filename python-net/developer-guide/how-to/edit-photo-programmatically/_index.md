---
type: docs
weight: '90'
url: /python-net/developer-guide/how-to/edit-photo-programmatically
linktitle: Edit photo or image programmatically
title: How to edit your photo or image programmatically
description: Library for image editing. Photo editing automation. Image manipulation by NET (Python) program. Removing photo background. Online photo editor.
keywords: [edit a photo, editing of pictures, edit an image, photo background editor, photo background change, resizing an image, resizing photos, photo sizing, picture resizer, image crop, crop photo, filter photo, online photo editor, online image editor, photo editing app, free photo editor]
---

## How to edit your photo or image programmatically

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Selling a unique product without effective advertising can be quite resourceful. This issue becomes even more evident in the realm of the Internet, where capturing a visitor's attention and maintaining their interest poses a real challenge. To illustrate this, let's draw a parallel between the online world and a real city. Imagine us strolling along streets, observing buildings, or driving in a car. Certainly, advertising stands out, whether it's the large banners decorating roads or the sophisticated posters promoting ongoing events. There was a time when such commercial posters became an art form, with famous artists using their skills for illustration. But everyone can afford the ability to produce high-quality images.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Aspose.Imaging library for Python .NET proves valuable for bulk image processing and repetitive image editing tasks required while preparing professional advertising materials, event posters, or even student projects. Frequently, the need to adjust source image characteristics like brightness, contrast, or gamma correction in readiness for subsequent publication. The library also facilitates the development of diverse applications or seamless integration into existing ones. For instance, it can be used to convert color images to black and white or grayscale or to provide an image watermarking service.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This article talks about how to use image editing tools with Aspose.Imaging Python library. If you want to see all the types of images this library can work with, look at the list of <a href="https://docs.aspose.com/imaging/python-net/supported-file-formats/">supported image formats</a>.
</p>


### Resizing an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Frequently, you have numerous raw images of varying sizes, and the need arises to standardize their widths while maintaining their width-to-length ratio for web placement. With Aspose.Imaging, you can automate the resizing of these images before publishing them. You simply need to specify the desired image width and apply it to the folder containing your raw images, while having the option to convert image formats simultaneously.
</p>

Python code examples: [howto resize image](resize-image).


### Crop an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Images might include uninteresting sections, or the main  might accidentally be positioned off-center within the photo. In such instances, the need to crop the images and eliminate undesired portions from the edges. Aspose.Imaging offers methods to facilitate image cropping by shifting and removing unwanted areas from the sides.
</p>

Python code example: [howto crop image](crop-image).


### Rotate

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In certain situations, you might encounter numerous photos that have been vertically or horizontally flipped, or rotated into incorrect orientations. Rotating each photo manually can be time-consuming but with the assistance of Aspose.Imaging, you can swiftly rotate or flip images collectively.
</p>

Python code example: [howto rotate image](rotate-image).


### Remove background

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
One of the most frequently requested image operations users often wish to perform is background removal. You might want to remove a human figure or another object from its surroundings. For complex images containing multiple elements, Aspose.Imaging offers various methods involving automatic or manual tagging of objects to facilitate background removal. Through the software library, you can define rectangular areas and preliminary label objects and their categories to enhance the precision of background removal.
</p>

Original image:

<img src="images/original_image.webp" alt="Original image before editing" width="640" height="427"/>

Image with removed background with assuming object method:

<img src="images/remove-background_auto.webp" alt="Image with removed background" width="640" height="427"/>

Python code example: [howto remove background](remove-background).


### Filter an image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can swiftly improve your photo's appearance by applying a range of filters to enhance sharpness or reduce noise. With the Aspose.Imaging Python library, you have the option to select from a diverse range of filters to apply captivating effects to an image, such as motion effects or blur filters.
</p>

Original image:

<img src="images/sample.webp" alt="Original image sample" width="640" height="480"/>

Image with Gauss blur filter applied:

<img src="images/gauss_blur_filter.webp" alt="Image with Gauss blur filter" width="640" height="480"/>

Python code example: [howto filter image](filter-image).


### Merge images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To craft collages comprising multiple images, you can leverage the merging function within Aspose.Imaging for Python. This feature allows you to position images adjacently, either horizontally or vertically, on the primary canvas. It's even possible to merge images of varying original formats, and subsequently save the resulting image in the desired new format.
</p>

Merged two images into one collage:

<img src="images/merge_images.webp" alt="Merged two images into one collage" width="640" height="240"/>

Python code example: [howto merge images](merge-images).


### Grayscale image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
One effective way to alter the perception of an image is by converting it to grayscale format. When color isn't a crucial factor, the absence of color can underscore the intrinsic essence of the picture. This force viewers to focus more on image details, as well as the interplay of light and shadow. Thanks to the Aspose Python library, you can effortlessly convert any image type into grayscale format.
</p>

Grayscaled image example:

<img src="images/Grayscaling_out.webp" alt="Image converted to Grayscale" width="640" height="480"/>

Python code example: [howto grayscale image](grayscale-image).


### Binarize image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A more profound transformation of images involves converting them into pure black and white, a process known as binarization. In this technique, every pixel is assigned one of two binary values: 1 (black) or 0 (white), with no intermediary grayscale gradation. This yields a striking image that is well-suited for applications such as posters or book illustrations. Aspose.Imaging offers a variety of methods to facilitate the creation of black-and-white images from color originals. These options encompass straightforward threshold techniques as well as more sophisticated methods that consider the values of neighboring pixels.
</p>

Example of black and image with binarization threshold 100:

<img src="images/BinarizationWithFixedThreshold_out.webp" alt="Image with binarize fixed threshold filter" width="640" height="480"/>

Python code example: [howto binarize image](binarize-image).


### Dither image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Image dithering is used for adding some noise to pictures. This method can increase image quality after reducing the color palette for publishing on the web and creating a trilling visual effect. With the Aspose image library, you use the simple `Threshold` method or the more complex `FloydSteinberg` method, which uses nearest neighbors’ pixels intensity values for dithering.
</p>

Example of image with `FloydSteinberg` dither method applied:

<img src="images/DitherImage_out.webp" alt="Dithered image for better quality" width="640" height="480"/>

Python code example: [howto dither image](dither-image).


### Adjust image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Adjusting image brightness, contrast and gamma are often used operations for image editing before publishing. Pictures may look pale or different areas of the image could be too darkened or too lighten without properly adjusting these parameters. These image defects lead to picture details loss and the general effect of a website with such images will be weak. You can perform brightness, contrast or gamma correction by passing appropriate parameters to the image library method.
</p>

Python code example: [howto adjust image](adjust-image).


### Drawing images

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
You can not only edit existing images but create new ones and draw various shapes such as Lines, Ellipses, Rectangles, Arcs and Bezier shapes. First, you need to create an image surface with selected background color, then select a tool Pen to draw with a specific brush, color and width.
</p>

Python code example: [howto drawing images](draw-image).


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
