---
title: Remove background from images
type: docs
weight: 80
url: /java/remove-background-from-images/
---

{{% alert color="primary" %}} 

Aspose.Imaging supports both manual and auto masking options for background removal from images.

{{% /alert %}} 

## **Auto Masking**
To receive better background removing results, Graph Cut segmentation with pre-calculated brushstrokes can be used.

### **Using Graph Cut auto masking with feathering**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. The Args property of AutoMaskingGraphCutOptions can be omitted since default strokes are placed there in the end.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-feathering.java" >}}

The figure below illustrates the result of the Graph Cut auto masking with feathering:

| {{< image img="remove-background_auto_1-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_1-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 2 (a) Original image                   | (b) Auto masked image                 |

### **Re-using default strokes in repeated auto masking with new points**

The following example demonstrates saving of the image masking results with feathering based on image size and re-using masking options for the new masking iteration. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions. After getting the initial masking results, applied background/foreground strokes are modified and another masking iteration is performed.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-repeated-masking-with-new-points.java" >}}

The figure below illustrates the result of re-using default strokes in repeated auto masking with new points:

| {{< image img="remove-background_auto_3-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_3-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 3 (a) Original image                   | (b) Auto masked image                   |

### **Using Graph Cut auto masking with specified assumed objects data**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. Additionally, the data of a one assumed human object is also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-assumed-objects-data.java" >}}

The figure below illustrates the result of the Graph Cut auto masking with specified assumed object data:

| {{< image img="remove-background_auto_4-1.jpg" alt="Original image" >}} | {{< image img="remove-background_auto_4-2.png" alt="Auto masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 4 (a) Original image                   | (b) Auto masked image                   |

## **Manual Masking**
The following code snippet provided below demonstrates how to apply manual masking to a raster image.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ManualImageMasking-ManualImageMasking.java" >}}

The figure below illustrates the result of the manual masking:

| {{< image img="remove-background_manual_1-1.jpg" alt="Original image" >}} | {{< image img="remove-background_manual_1-2.png" alt="Manually masked image" >}} |
| ------------------------------------------- | ------------------------------------------- |
| Fig. 5 (a) Original image                   | (b) Manually masked image                   |


