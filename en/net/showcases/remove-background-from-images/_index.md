---
title: Remove background from images
type: docs
weight: 80
url: /net/remove-background-from-images/
---

{{% alert color="primary" %}} 

Aspose.Imaging supports both manual and auto masking options for background removal from images.

{{% /alert %}} 

## **Auto Masking**
To receive better background removing results, Graph Cut segmentation with pre-calculated brushstrokes can be used.

### **Graph Cut auto masking using Imaging.Cloud API**

The following example demonstrates usage of the Imaging.Cloud API's detected objects as an input for Graph Cut auto masking to further improve masking results. DetectedObjectList's data is converted into an AssumedObjectData collection first so that it can be passed into the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-using-object-detection-from-cloud.cs" >}}

The figure below illustrates the result of the Graph Cut auto masking using Imaging.Cloud API:

| {{< image img="remove-background_auto_1-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_1-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 1 (a) Original image                   | (b) Auto masked image                   |

### **Using Graph Cut auto masking with feathering**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. The Args property of AutoMaskingGraphCutOptions can be omitted since default strokes are placed there in the end.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-feathering.cs" >}}

The figure below illustrates the result of the Graph Cut auto masking with feathering:

| {{< image img="remove-background_auto_2-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_2-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 2 (a) Original image                   | (b) Auto masked image                 |

### **Re-using default strokes in repeated auto masking with new points**

The following example demonstrates saving of the image masking results with feathering based on image size and re-using masking options for the new masking iteration. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions. After getting the initial masking results, applied background/foreground strokes are modified and another masking iteration is performed.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-repeated-masking-with-new-points.cs" >}}

The figure below illustrates the result of re-using default strokes in repeated auto masking with new points:

| {{< image img="remove-background_auto_3-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_3-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 3 (a) Original image                   | (b) Auto masked image                   |

### **Using Graph Cut auto masking with specified assumed objects data**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. Additionally, the data of a one assumed human object is also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "graph-cut-assumed-objects-data.cs" >}}

The figure below illustrates the result of the Graph Cut auto masking with specified assumed object data:

| {{< image img="remove-background_auto_4-1.jpg" alt="Original image">}} | {{< image img="remove-background_auto_4-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 4 (a) Original image                   | (b) Auto masked image                   |

## **Manual Masking**
The following code snippet provided below demonstrates how to apply manual masking to a raster image.

{{< gist "aspose-com-gists" "cd4fed97fcdfa3055fbffc65e5298664" "manual-image-masking.cs" >}}

The figure below illustrates the result of the manual masking:

| {{< image img="remove-background_manual_1-1.jpg" alt="Original image" >}} | {{< image img="remove-background_manual_1-2.png" alt="Manually masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 5 (a) Original image                   | (b) Manually masked image                   |


