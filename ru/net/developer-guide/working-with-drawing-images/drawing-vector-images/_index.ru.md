---
title: Drawing Vector Images
type: docs
weight: 50
url: /ru/net/drawing-vector-images/
---





{{% alert color="primary" %}} 

Drawing a vector image is not supported at now. It needs to convert the drawn vector image to a raster before drawing.

{{% /alert %}} 
## **Draw Vector Image**
Using Aspose.Imaging for .NET you can draw vector image on another vector image. With a few simple steps, you will be able to draw a vector image on another vector image.

- Create MemoryStream object
- Load a SVG image
- Rasterize SVG to PNG and write the result to a stream
- Load a PNG image from stream for further drawing
- Draw PNG image on existing SVG image
- Save the results



{{< gist "aspose-com-gists" "fb30abde0bc8795ce6828496afc29b42" "draw-vector-image-to-raster-image.cs" >}}
