---
title: Drawing Images using Graphics
type: docs
weight: 20
url: /python-net/drawing-images-using-graphics/
---

## **Drawing Images using Graphics**
With the Aspose.Imaging library you can draw simple shapes like lines, rectangles and circles, as well as complex shapes like polygons, curves, arcs and Bezier shapes. Aspose.Imaging library creates such shapes using [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) class that resides in the aspose.imaging namespace. Graphics objects are responsible for performing different drawing operations on an image, thus changing the image's surface. The Graphics class uses a variety of helper objects to enhance the shapes:

- Pens, to draw lines, outline shapes, or render other geometric representations.
- Brushes, to define how areas are filled in.
- Fonts, to define the shape of characters of text.

### **Drawing with the Graphics Class**
Below is a code example demonstrating the use of the [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) class. The example source code has been split into several parts to keep it simple and easy to follow. Step by step, the examples show how to:

1. Create an image.
1. Create and initialize a [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) object.
1. Clear the surface.
1. Draw an ellipse.
1. Draw a filled polygon and save the image.

### **Programming Samples**
#### **Creating an Image**
Start by creating an image using any of the methods described in [Creating Files](https://docs.aspose.com/imaging/python-net/drawing-images/#DrawingandFormattingImages-CreatingImageFiles).

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-lines.py" >}}

#### **Create and Initialize a Graphics Object**
Then create and initialize a [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) object by passing the [Image](https://reference.aspose.com/imaging/python-net/aspose.imaging/image) object to its constructor.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-rectangle.py" >}}

#### **Clear the Surface**
Clear the [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) surface by calling the Graphics class [clear](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics/#methods) method and pass a color as a parameter. This method fills the Graphics surface with the color passed in as argument.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-arc.py" >}}

#### **Draw an Ellipse**
You may notice that the [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) class has exposed plenty of methods to draw and fill shapes. You'll find get the complete list of methods in the [Aspose.Imaging for Python via .NET API Reference](https://docs.aspose.com/imaging/python-net/crop-rotate-and-resize-images/). There are several overloaded versions of the [draw_ellipse](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics/#methods) method exposed by the Graphics class. All these methods accept a [Pen](https://reference.aspose.com/imaging/python-net/aspose.imaging/pen) object as its first argument. The later parameters are passed to define the bounding rectangle around the ellipse. For the sake of this example, use the version accepting a [Rectangle](https://reference.aspose.com/imaging/python-net/aspose.imaging/rectangle) object as the second parameter to draw an ellipse using the [Pen](https://reference.aspose.com/imaging/python-net/aspose.imaging/pen) object in your desired color.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-ellipse.py" >}}

#### **Draw a Filled Polygon**
Next, draw a polygon using the LinearGradientBrush and an array of points. The [Graphics](https://reference.aspose.com/imaging/python-net/aspose.imaging/graphics) class has exposed several overloaded versions of the fill_polygon() method. All of these accept a Brush object as its first argument, defining the characteristics of the fill. The second parameter is an array of points. Please note that every two consecutive points in the array specify a side of the polygon.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-filled-polygon.py" >}}

#### **Measure string using Aspose.Graphics**
Aspose.Imaging Graphics supports method to measure string. Here the sample code for it is provided.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "graphics-measure-string.py" >}}

### **Drawing Images using Graphics : Complete Source**
{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "drawing-using-graphics.py" >}}

All classes that implement __enter__ and __exit__ methods and access unmanaged resources are instantiated in a **with** statement to ensure that they are disposed of correctly.

### **Drawing Text on images using Graphics**
Using Aspose.Imaging you can easily draw text on image with text alignment using Graphics.
{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "draw-text-using-graphics.py" >}}

## **Memory Strategy optimization**
Graphics operations can be proceeded using memory strategy optimization - ie limiting memory buffer size for operation.

{{< gist "aspose-com-gists" "040f3eed820b297360357d5e45066036" "memory-strategy-optimization.py" >}}
