---
title: Drawing Images using GraphicsPath
type: docs
weight: 30
url: /net/drawing-images-using-graphicspath/
---

## **Drawing Images using GraphicsPath**
The [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) class is responsible for creating and maintaining a graphics path. The GraphicsPath has no reference to an image and does not change the image itself, instead, it can be considered as an object that contains metadata that describes the paths that [Graphics](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) class can draw. The GraphicsPath class uses figures; each figure is either composed of a sequence of connected lines and curves or a geometric shape primitive. Each shape may be split into shape segments. You can add, remove and change different figures or shapes in a GraphicsPath object. When the GraphicsPath has been fully described, use the corresponding Graphics class methods (DrawPath and [Fill Paths](https://reference.aspose.com/imaging/net/aspose.imaging/graphics/methods/fillpath) to draw over or fill the paths. The Graphics class takes each shape segment and draws it to produce the final image.
### **Drawing using GraphicsPath Class**
Below is an example demonstrating the use of the [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) class. The example source code has been split in several parts to keep it simple and easy to follow. Step by step, the examples show you how to:

1. Create an image.
1. Initialize a [Graphics](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) object.
1. Clear the surface.
1. Create an instance of [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath).
1. Create a figure.
1. Add shapes to the figure.
1. Create a Figures array.
1. Draw paths.
1. Fill paths.
### **Drawing Images using GraphicsPath: Programming Samples**
#### **GraphicsPath : Create an Image**
Start by creating an image using any of the methods described in [Creating Files](https://docs.aspose.com/imaging/net/drawing-images/#DrawingandFormattingImages-CreatingImageFiles).

{{< gist "aspose-com-gists" "a582f56501be0db2329593b3908ee49d" "drawing-lines.cs" >}}


#### **GraphicsPath : Initialize a Graphics Objects**
Create and initialize a [Graphics](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) object by passing the [Image](https://reference.aspose.com/imaging/net/aspose.imaging/image) object to its constructor.

{{< gist "aspose-com-gists" "a582f56501be0db2329593b3908ee49d" "drawing-rectangle.cs" >}}


#### **GraphicsPath : Clear the Surface**
Clear the [Graphics](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) surface by calling the Graphics class [Clear](https://reference.aspose.com/imaging/net/aspose.imaging/graphics/methods/clear) method and pass a Color as a parameter. This method fills the Graphics surface with the color passed in as argument.

{{< gist "aspose-com-gists" "a582f56501be0db2329593b3908ee49d" "drawing-arc.cs" >}}


#### **GraphicsPath : Create an Instance of the GraphicsPath**
Create an instance of [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) with [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) set to **Alternate** by default. This mode determines how to fill the interior of a closed figure. The other possible [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) value is **Winding**.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "create-graphics-path-wth-shapes-and-figures.cs" >}}


#### **GraphicsPath : Create a Figure**
Create an instance of the [Figure](https://reference.aspose.com/imaging/net/aspose.imaging/figure) class. As discussed earlier, [Figure](https://reference.aspose.com/imaging/net/aspose.imaging/figure) can contain Shapes and shapes reside in the [Aspose.Imaging.Shapes](http://www.aspose.com/docs/display/imagingnet/Aspose.Imaging.Shapes+namespace) namespace.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "create-graphics-path-wth-shapes-and-figures.cs" >}}


#### **GraphicsPath : Add Shapes to the Figure**
The [Add Shapes](https://reference.aspose.com/imaging/net/aspose.imaging/figure/methods/addshapes) method exposed by the [Figure](https://reference.aspose.com/imaging/net/aspose.imaging/figure) class lets you add shapes to the figure. In the code examples below, several shapes are added to a Figure object.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "create-graphics-path-wth-shapes-and-figures.cs" >}}


#### **GraphicsPath : Add Figures to an Array**
Multiple figures can be added to a [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) object using the AddFigures method exposed by the GraphicsPath class. This method accepts an array of figures as a parameter.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "create-graphics-path-wth-shapes-and-figures.cs" >}}


#### **GraphicsPath : Draw the Paths**
Draw the [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) using the DrawPath method exposed by Graphics class. The method accepts two parameters. The first parameter is an object of the [Pen](https://reference.aspose.com/imaging/net/aspose.imaging/pen) class, which determines the color, width and style of the path. The second parameter is the object of the GraphicsPath class, representing the path itself.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "create-graphics-path-wth-shapes-and-figures.cs" >}}


#### **GraphicsPath : Fill Paths**
You can fill a path by passing a [GraphicsPath](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) object to the [Fill Paths](http://www.aspose.com/api/net/imaging/aspose.imaging/graphics/methods/fillpath) method exposed by the [Graphics](https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath) class. The [Fill Paths](http://www.aspose.com/api/net/imaging/aspose.imaging/graphics/methods/fillpath) method fills the path according to the fill mode (alternate or winding) currently set for the path. If the path has any open figures, the path is filled as if those figures were closed.

The [Fill Paths](http://www.aspose.com/api/net/imaging/aspose.imaging/graphics/methods/fillpath) method accepts two parameters. The first parameter is an object of any brush class from the [Aspose.Imaging.Brushes](http://www.aspose.com/docs/display/imagingnet/Aspose.Imaging.Brushes+namespace) namespace. The second parameter is the path itself. For the sake of this example, use the HatchBrush which is a rectangular brush with a hatch style, a foreground color, and a background color. Before passing the HatchBrush object to the [Fill Paths](http://www.aspose.com/api/net/imaging/aspose.imaging/graphics/methods/fillpath) method, set its properties.

{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "fill-graphics-path.cs" >}}


### **GraphicsPath : Complete Source**
{{< gist "aspose-com-gists" "8b7ada69bad4dc49dac0b9f4f5cc8329" "drawing-using-graphics-path.cs" >}}


All classes that implements IDisposable are instantiated in a Using statement to ensure that they are disposed of correctly.
