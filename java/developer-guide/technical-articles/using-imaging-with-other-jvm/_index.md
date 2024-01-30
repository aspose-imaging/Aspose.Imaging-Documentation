---
title: Using Aspose.Imaging for all JVMs and Platforms
type: docs
weight: 100
url: /java/using-imaging-with-other-jvm/
description: Explore the diverse capabilities of the Aspose.Imaging for Java library, designed to seamlessly integrate across various Java Virtual Machines (JVM) and supported JDK
keywords: Java, JDK, JVM, GraalVM, Aspose.Imaging for Java, Java API, image processing, imaging library, GraalVM integration, Oracle JDK, OpenJDK, Amazon Corretto integration, Eclipse Temurin integration, Red Hat OpenJDK integration, image processing applications, create and manipulate images
---

## Aspose.Imaging Library's Cross-Platform Versatility

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The Aspose.Imaging for Java library is versatile across various Java Virtual Machines (JVM). You can leverage its flexibility to develop image processing applications and services using various Java Development Kits (JDK), whether proprietary or open licenses and deploy them across diverse platforms and operating systems.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Initially developed by Sun and later by Oracle, Java components were open-sourced. Now, it forms a diverse Java ecosystem spanning multiple platforms, facilitating true cross-platform development and deployment. Regardless of your preferred operating system — be it Windows, Linux, or MacOS — you can utilize any available JDK to compile Java classes for the JVM using both ahead-of-time (AOT) and just-in-time (JIT) techniques for enhanced performance. Your application can incorporate the Aspose.Imaging for Java API to create and manipulate images, ensuring consistently reliable results.
</p>

List of supported platforms:

- Graal JVM
- Oracle JDK 8
- Oracle JDK 17
- Oracle JDK 21
- OpenJDK 8
- Azul Platform Core
- Amazon Corretto
- Eclipse Temurin
- Red Hat OpenJDK

Supported OS:

- Windows
- Linux
- MacOS (x64, arm64)

## Seamless Integration with GraalVM/OpenJDK

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
GraalVM, a modern JVM implementation written in Java with AOT and JIT support, is built upon the Oracle HotSpot JVM and OpenJDK. You can easily integrate Aspose.Imaging library to this platform. To execute your Java application with the Aspose imaging library on GraalVM, download GraalVM from the official site and create a batch file with the necessary links to the JVM. For Windows users, here is an example of a `start.bat` file:
</p>

```sh
@echo off
setlocal
set JAVA_HOME=C:\ManualSoft\graalvm-community-openjdk-21+35.1
set PATH=C:\ManualSoft\graalvm-community-openjdk-21+35.1\bin;%PATH%

"%JAVA_HOME%\bin\java" -cp "filename.jar;" <classname>
```

The last version of Aspose.Imaging for Java library you can download from the  <a href="https://releases.aspose.com/java/repo/com/aspose/aspose-imaging/">Aspose maven repository</a>. Please follow Aspose.Imaging <a href="https://docs.aspose.com/imaging/java/installation/">Installation instructions</a>. 
