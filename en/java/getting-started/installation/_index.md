---
title: Installation
type: docs
weight: 40
url: /java/installation/
description: Java Image Processing Library or API can be installed through Maven.
---

## **Installing Aspose.Imaging for Java from Maven Repository**
Aspose hosts all Java APIs on [Maven repository](https://repository.aspose.com/repo/com/aspose/). You can easily use [Aspose.Imaging for Java](https://repository.aspose.com/repo/com/aspose/aspose-imaging/) API directly in your Maven Projects with simple configurations.
### **Specify Maven Repository Configuration**
First you need to specify Aspose Maven Repository configuration / location in your Maven pom.xml as follows:

{{< highlight xml >}}

 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>

{{< /highlight >}}
### **Define Aspose.Imaging for Java API Dependency**
Then define Aspose.Imaging for Java API dependency in your pom.xml as follows:

{{< highlight xml >}}

 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-imaging</artifactId>
        <version>23.10</version>
        <classifier>jdk16</classifier>
   </dependency>

   <!-- if you need a documentation, please add the following dependency. For example it could be useful for IDE. -->
   <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-imaging</artifactId>
        <version>23.10</version>
        <classifier>javadoc</classifier>
   </dependency>
</dependencies>

{{< /highlight >}}

After performing above steps, Aspose.Imaging for Java dependency will finally be defined in your Maven Project.
