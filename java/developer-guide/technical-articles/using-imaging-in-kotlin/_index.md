---
title: Using Aspose.Imaging for Java in Kotlin
type: docs
weight: 100
url: /java/using-imaging-in-kotlin/
description: How to use Aspose.Imaging for Java in Kotlin applications for desktops and servers
keywords: Kotlin applications, Aspose.Imaging for Java, export svg to png in Kotlin, create images in Kotlin, modify images in Kotlin, load images in Kotlin, save images in Kotlin, crop image in Kotlin, merge images in Kotlin
---

## **Using Aspose.Imaging for Java in Kotlin Applications**

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the dynamic landscape of software development, the synergy between programming languages is a powerful force. Kotlin, known for its conciseness and interoperability with Java, opens doors for developers seeking to enhance their applications with sophisticated features. The Aspose.Imaging graphic library is applicable for both desktop and server applications. For now, it does not support the Android platform, but support for it will be included in the upcoming releases.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
This article delves into the realm of Aspose.Imaging for Java and how seamlessly it integrates with Kotlin applications. We will explore the capabilities, advantages, and practical implementation of using Aspose.Imaging in Kotlin projects. This guide will provide you with knowledge on how to use the power of the image library for enriched visual experiences in your applications.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To start using Aspose.Imaging in your project, add dependency to the Gradle file `build.gradle.kts`:
</p>

```groovy
repositories {
    mavenCentral()
    maven {
        url = uri("https://repository.aspose.com/repo/")
    }
}
// ....................
dependencies {
   //... some code
   implementation(group="com.aspose", name="aspose-imaging", version = "23.11"
        , classifier = "jdk16")
   //... some code
}
```

## **Examples**

### Create a new PNG image, draw a line on it and save it

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In the Kotlin code snippet below, we demonstrate the creation of a PNG image, drawing geometric figures, and applying resizing and cropping transformations. In this example, we initiate the creation of a PNG image with a size of 500x300 pixels and a green background. Subsequently, we draw a blue line on the image using a `Pen` object. Before saving the image, we apply resizing to a width of 400 pixels and crop it to a specific rectangle area. All method descriptions you find in the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/">official API reference site</a>.
</p>

```java
import com.aspose.imaging.Color
import com.aspose.imaging.Graphics
import com.aspose.imaging.Image
import com.aspose.imaging.Pen
import com.aspose.imaging.Rectangle
import com.aspose.imaging.ResizeType
import com.aspose.imaging.fileformats.png.PngImage
import com.aspose.imaging.imageoptions.PngOptions
import com.aspose.imaging.sources.FileCreateSource

fun createAndSave() {
    // Image width
    val width = 500
    // Image height
    val height = 300

    // Where created image to store
    val path = "C:\\createdImage.png"

    // Create options
    val options = PngOptions()
    options.source = FileCreateSource(path, false)

    (Image.create(options, width, height) as PngImage).use { image ->
        // Create and initialize an instance of Graphics class
        val graphic = Graphics(image)
        // and Clear Graphics surface
        graphic.clear(Color.getGreen())
        // Draw line on image
        graphic.drawLine(Pen(Color.getBlue()), 9, 9, 90, 90)

        // Resize image
        val newWidth = 400
        image.resizeWidthProportionally(newWidth, ResizeType.LanczosResample)

        // Crop the image to specified area
        val area = Rectangle(10, 10, 200, 200)
        image.crop(area)
        // save in default path
        image.save()
    }
}
```

### Load, resize and save a raster image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Let's dive into a real scenario where we load a TIFF image, resize it, and save the transformed image in JPEG format using Kotlin. In this example, we begin by importing the necessary Aspose.Imaging classes. We then load a TIFF image using `Image.load()`. After loading the image, we resize it to half of its original size with the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/image/#resize-int-int-">resize()</a> method. Finally, we save the resized image in JPEG format using the `save()` method.
</p>

```java
import com.aspose.imaging.Image

// load TIFF
(Image.load("any-picture.tiff")).use { image ->
        image.resize(image.width / 2, image.height / 2)
        // and save as JPEG
        image.save("output.jpeg")
}
```

### Load JPEG and export it into different formats

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Additionally, you have the flexibility to load images in Kotlin, like JPEG files, and then convert them to various other formats, including WEBP, PSD, TIFF (Black and White), or TIFF (RGBA color space with a transparency alpha layer):
</p>

```java
import com.aspose.imaging.Image
import com.aspose.imaging.fileformats.pdf.PdfDocumentInfo
import com.aspose.imaging.fileformats.tiff.enums.TiffExpectedFormat
import com.aspose.imaging.imageoptions.PdfOptions
import com.aspose.imaging.imageoptions.PsdOptions
import com.aspose.imaging.imageoptions.TiffOptions
import com.aspose.imaging.imageoptions.WebPOptions

val dir = "C:\\Temp\\";
Image.load(dir + "template.jpg").use { img ->
    // save in different formats
    img.save(dir + "output.webp", WebPOptions())
    img.save(dir + "output.psd ", PsdOptions())
    // save in B/W TIFF
    img.save(dir + "output.tiff", TiffOptions(TiffExpectedFormat.Default))
    // save in ARGB TIFF
    img.save(dir + "output.tiff", TiffOptions(TiffExpectedFormat.TiffDeflateRgba))

    // Save image to Pdf
    val exportOptions = PdfOptions()
    exportOptions.pdfDocumentInfo = PdfDocumentInfo()
    img.save(dir + "output.pdf", exportOptions)
}
```

### Crop image

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To crop images in Kotlin, utilize the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/rasterimage/#crop-com.aspose.imaging.Rectangle-">rasterImage.crop()</a> method with a specified Rectangle area:
</p>

```java
import com.aspose.imaging.Image
import com.aspose.imaging.RasterImage
import com.aspose.imaging.Rectangle

val dataDir = "C:\\Temp\\"
(Image.load(dataDir + "template.jpg")).use { img ->
    // casting to the RasterImage class
    val rasterImage = img as RasterImage
    // crop
    val area = Rectangle(10, 10, img.width - 20, img.height - 20)
    rasterImage.crop(area)
    img.save("cropped.jpg")
}
```

### Merge images into one (collage)

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
With Aspose.Imaging, you can seamlessly merge multiple images into one to create a collage using the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging/graphics/#drawImage-com.aspose.imaging.Image-com.aspose.imaging.RectangleF-">graphics.drawImage() method</a>. You have the flexibility to choose between vertical or horizontal image placement directions and select background colors according to your preference:
</p>

```java
import com.aspose.imaging.Color
import com.aspose.imaging.Graphics
import com.aspose.imaging.Image
import com.aspose.imaging.RectangleF
import com.aspose.imaging.fileformats.png.PngColorType
import com.aspose.imaging.imageoptions.PngOptions
import com.aspose.imaging.sources.StreamSource
import java.io.File

internal enum class MergeStyle {
    Horizontal,
    Vertical
}

fun collage() {
    // Test directory should have source images to merge
    val TestDirectory = "D:\\Many2One\\"
    val mStyle = MergeStyle.Horizontal // or MergeStyle.Vertical

    val images = mutableListOf<Image>()
    try {
        var totalWidth = 0
        var totalHeight = 0
        var maxWidth = 0
        var maxHeight = 0

        val fileMask = ".png"
        val files = File(TestDirectory).listFiles { dir, name -> name.endsWith(fileMask) } ?: return

        for (fileName in files) {
            Image.load(fileName.absolutePath).use { image ->
                totalWidth += image.width
                if (image.width > maxWidth) {
                    maxWidth = image.width
                }
                totalHeight += image.height
                if (image.height > maxHeight) {
                    maxHeight = image.height
                }
                images.add(image)
            }
        }

        if (images.isEmpty()) {
            return
        }

        var mergeStyle: String
        val targetWidth: Int
        val targetHeight: Int
        if (mStyle === MergeStyle.Horizontal) {
            targetWidth = totalWidth
            targetHeight = maxHeight
        } else if (mStyle === MergeStyle.Vertical) {
            targetWidth = maxWidth
            targetHeight = totalHeight
        } else {
            return  // other merge styles are not supported
        }

        var outputPath = TestDirectory + "output\\"
        val dir = File(outputPath)
        assert(dir.exists() || dir.mkdirs())
        outputPath = outputPath + "merged_" + mStyle.name + ".png"
        val pngOptions = PngOptions()
        pngOptions.colorType = PngColorType.TruecolorWithAlpha
        pngOptions.source = StreamSource()
        Image.create(pngOptions, targetWidth, targetHeight).use { image ->
            image.backgroundColor = Color.getWhite()
            val graphics = Graphics(image)
            var x = 0f
            var y = 0f
            for (it in images) {
                graphics.drawImage(it, RectangleF(x, y, it.width.toFloat(), it.height.toFloat()))
                if (mStyle === MergeStyle.Horizontal) {
                    x += it.width.toFloat()
                }
                if (mStyle === MergeStyle.Vertical) {
                    y += it.height.toFloat()
                }
            }
            image.save(outputPath)
        }
    }
    finally {
        for (image in images) {
            image.close()
        }

        images.clear()
    }
}
```

### Export vector image in SVG format to PNG

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Using Imaging goes beyond raster images; you can also convert vector images, such as SVG, into PNG. Employ the <a href="https://reference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/svgrasterizationoptions/">imageoptions.SvgRasterizationOptions class</a> to seamlessly export SVG to a raster image format.
</p>

```java
import com.aspose.imaging.Image
import com.aspose.imaging.imageoptions.PngOptions
import com.aspose.imaging.imageoptions.SvgRasterizationOptions
import java.io.File

// get path of the input data
var templatesFolder = System.getenv("DATA_PATH")
// get output path
var outputFolder = System.getenv("OUT_PATH")

if (templatesFolder == null) templatesFolder = "data"

if (outputFolder == null) outputFolder = "out"

// Load the svg file in an instance of Image
Image.load(templatesFolder + File.separator + "template.svg").use { image ->
    // Create an instance of PngOptions
    val exportOptions = PngOptions()
    val vectorOptions = SvgRasterizationOptions()
    vectorOptions.pageWidth = image.width.toFloat()
    vectorOptions.pageHeight = image.height.toFloat()
    exportOptions.vectorRasterizationOptions = vectorOptions

    // Save svg to png
    image.save(outputFolder + File.separator + "svg-to-png-output.png", exportOptions)
}
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Join us on this journey where Kotlin and Java converge to elevate the Aspose.Imaging capabilities of your software projects. Download the last version of Aspose.Imaging for Java from the <a href="https://releases.aspose.com/imaging/java/">official release site</a>.
</p>
