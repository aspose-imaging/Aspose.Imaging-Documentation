---
title: Remove background from images
type: docs
weight: 10
url: /java/removing-background-from-images/
---

{{% alert color="primary" %}} 

Masking involves setting some of the pixel values in an image to zero, or some other "background" value. Aspose.Imaging supports the following types of masking.

- Manual Masking
- Auto Masking

{{% /alert %}} 

## **Auto Masking**

### **Using Graph Cut auto masking with feathering**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. The Args property of AutoMaskingGraphCutOptions can be omitted since default strokes are placed there in the end.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-feathering.java" >}}

### **Re-using default strokes in repeated auto masking with new points**

The following example demonstrates saving of the image masking results with feathering based on image size and re-using masking options for the new masking iteration. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions. After getting the initial masking results, applied background/foreground strokes are modified and another masking iteration is performed.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-repeated-masking-with-new-points.java" >}}

### **Using Graph Cut auto masking with specified assumed objects data**

The following example demonstrates saving of the image masking results with feathering based on image size. Image masking is performed using auto calculated default strokes. Additionally, the data of the two assumed objects are also specified in the AssumedObjects property of the AutoMaskingGraphCutOptions.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-assumed-objects-data.java" >}}

### **Performing Graph Cut segmentation with user-defined point and feathering radius**
The following example demonstrates saving of the Graph Cut image masking result with feathering set to 3. Image masking is performed using the user-defined Point array.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-graph-cut-user-defined-point-and-feathering-radius.java" >}}

The following code snippet provided below demonstrates how to apply auto masking to a raster image.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-AutoImageMasking.java" >}}

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-FillInputPoints.java" >}}

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-LEIntegerReader.java" >}}

## **Manual Masking**
The following code snippet provided below demonstrates how to apply manual masking to a raster image.

{{< gist "aspose-com-gists" "07be292db0a393dc95f153f84b28c069" "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ManualImageMasking-ManualImageMasking.java" >}}

