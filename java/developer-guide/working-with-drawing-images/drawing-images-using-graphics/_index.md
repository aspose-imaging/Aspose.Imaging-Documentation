---
title: Drawing Images using Graphics
type: docs
weight: 20
url: /java/drawing-images-using-graphics/
---

## **Drawing Images using Graphics**
With the Aspose.Imaging library you can draw simple shapes like lines, rectangles and circles, as well as complex shapes like polygons, curves, arcs and Bezier shapes. Aspose.Imaging library creates such shapes using [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class that resides in the com.aspose.imaging package. Graphics objects are responsible for performing different drawing operations on an image, thus changing the image's surface. The [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class uses a variety of helper objects to enhance the shapes:

- Pens, to draw lines, outline shapes, or render other geometric representations.
- Brushes, to define how areas are filled in.
- Fonts, to define the shape of characters of text.
### **Drawing with the Graphics Class**
Below is a code example demonstrating the use of the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class. The example source code has been split into several parts to keep it simple and easy to follow. Step by step, the examples show how to:

1. Create an image.
1. Create and initialize a [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) object.
1. Clear the surface.
1. Draw an ellipse.
1. Draw a filled polygon and save the image.
### **Programming Samples**
#### **Creating an Image**
Start by creating an image using any of the methods described in ["Creating Opening and Saving Images"](/imaging/java/creating-opening-and-saving-images/).

#### **Create and Initialize a Graphics Object**
Then create and initialize a [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) object by passing the [Image](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image) object to its constructor.

#### **Clear the Surface**
Clear the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) surface by calling the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class [clear](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#clear-com.aspose.imaging.Color-) method and pass a color as a parameter. This method fills the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) surface with the color passed in as argument.

#### **Draw an Ellipse**
You may notice that the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class has exposed plenty of methods to draw and fill shapes. You'll find get the complete list of methods in the [Aspose.Imaging for Java API Reference](https://apireference.aspose.com/imaging/java). There are several overloaded versions of the [drawEllipse](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#drawEllipse-com.aspose.imaging.Pen) method exposed by the [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class. All these methods accept a [Pen](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Pen) object as its first argument. The later parameters are passed to define the bounding rectangle around the ellipse. For the sake of this example, use the version accepting a [Rectangle](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Rectangle) object as the second parameter to draw an ellipse using the [Pen](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Pen) object in your desired color.

#### **Draw a Filled Polygon**
Next, draw a polygon using the [LinearGradientBrush ](https://apireference.aspose.com/imaging/java/com.aspose.imaging.brushes/LinearGradientBrush) and an array of points. The [Graphics](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics) class has exposed several overloaded versions of the [fillPolygon](https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#fillPolygon-com.aspose.imaging.Brush-com.aspose.imaging.Point:A-) method. All of these accept a Brush object as its first argument, defining the characteristics of the fill. The second parameter is an array of points. Please note that every two consecutive points in the array specify a side of the polygon.

#### **Measure string using Aspose.Graphics**
Aspose.Imaging Graphics supports method to measure string. Here the sample code for it is provided.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graphics-measure-string.java" >}}

### **Drawing Images using Graphics : Complete Source**
All classes that implement Closeable interface and access unmanaged resources are instantiated in the try-with-resources or try-finally statements to ensure that they are disposed of correctly.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-images-DrawingusingGraphics-DrawingusingGraphics.java" >}}

### **Drawing Text on images using Graphics**
Using Aspose.Imaging you can easily draw text on image with text alignment using Graphics.

{{< gist "aspose-com-gists" "c8d164b9aaf58702d431710fe0181ced" "draw-text-using-graphics.java" >}}

## **Memory Strategy optimization**
Graphics operations can be proceeded using memory strategy optimization - i.e. limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "MemoryStrategyOptimizationGraphics.java" >}}
