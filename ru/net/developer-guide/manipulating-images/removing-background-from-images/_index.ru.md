---
title: Remove background from images in C#
linktitle: Remove background from images
type: docs
weight: 10
url: /ru/net/removing-background-from-images/
description: Setting some of the pixel values in an image to zero, or some other “background” value is known as Masking. C# Image Processing Library supports the following types of masking.
---

{{% alert color="primary" %}} 

Masking involves setting some of the pixel values in an image to zero, or some other "background" value. Aspose.Imaging supports the following types of masking.

- Manual Masking
- Auto Masking

{{% /alert %}} 

## **Auto Masking**
### **Graph Cut auto masking using Imaging.Cloud API**

To get better remove background results, Graph Cut segmentation with pre-calculated brushstrokes can be used. The following example demonstrates usage of the Imaging.Cloud API's detected objects as an input for Graph Cut auto masking to further improve masking results. DetectedObjectList's data is converted into an AssumedObjectData collection first so that it can be passed into the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-using-object-detection-from-cloud.cs" >}}

### **Using Graph Cut auto masking with feathering**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. The Args property of AutoMaskingGraphCutOptions can be omitted since default strokes are placed there in the end.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-feathering.cs" >}}

### **Re-using default strokes in repeated auto masking with new points**

The following example demonstrates saving of the image masking results with feathering based on image size and re-using masking options for the new masking iteration. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions. After getting the initial masking results, applied background/foreground strokes are modified and another masking iteration is performed.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-repeated-masking-with-new-points.cs" >}}

### **Using Graph Cut auto masking with specified assumed objects data**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-assumed-objects-data.cs" >}}

### **Performing Graph Cut segmentation with user-defined point and feathering radius**
The following example demonstrates saving of the Graph Cut image masking result with feathering set to 3. Image masking is performed using the user-defined Point array.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-user-defined-point-and-feathering-radius.cs" >}}

The following code snippet provided below demonstrates how to apply auto masking to a raster image.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "auto-image-masking.cs" >}}

## **Manual Masking**
The following code snippet provided below demonstrates how to apply manual masking to a raster image.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "manual-image-masking.cs" >}}




