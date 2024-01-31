---
title: Create Binary App with Graal Native Image
type: docs
weight: 100
url: /java/create-binary-app-with-graal-native-image/
description: How Graal Native Image technology empowers developers to compile high-performance Aspose.Imaging binary programs, offer fast application starts and efficient image processing.
keywords: Aspose.Imaging for Java, Java Virtual Machine, JVM, GraalVM, Native image, native binary, ahead-of-time, image creation, image manipulation, image effects, image processing, compile bytecode, platform independence
---

## Exploring Java's Evolution: Platform Independence and Trade-offs

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Sun Microsystems initially introduced Java technology with the primary objective of compiling programs into a special bytecode, executed on the platform-independent Java Virtual Machine (JVM). This enables developers to create programs in Java and execute the compiled bytecode on any operating system where the JVM is available, including Windows, MacOS, Linux, and others. While this approach offers platform independence, it comes with certain trade-offs. Platform-independent applications may experience increased starting time latency, higher memory usage, and generally slower program execution compared to native binary compiled code. Although modern hardware has alleviated many of these drawbacks, there are cases where execution speed remains a consideration.
</p>

## Leveraging Native Image Technology for High-Efficiency Aspose.Imaging in Java

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
GraalVM Native Image technology empowers Java developers to compile Java code ahead-of-time (AOT) into a platform-dependent native binary, complete with an embedded Java runtime. This resulting binary functions as a standalone executable, tailored for the target platform. Leveraging this method facilitates the creation of high-performance Aspose.Imaging programs for image creation and manipulations. The outcome is an Aspose.Imaging application that starts within milliseconds and efficiently processes images and photos, applying image effects and filters while utilizing fewer system resources.
</p>

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
To generate a native binary from Java code using the Aspose.Imaging library, compile Java classes to bytecode, and subsequently compile it to binary using the GraalVM `native-image` utility:
</p>

```sh
javac Aspose.Imaging-example.java
native-image Aspose.Imaging-example
```

You can find the latest version of Aspose.Imaging for Java library in official <a href="https://releases.aspose.com/java/repo/com/aspose/aspose-imaging/">Aspose maven repository</a>. Please follow Aspose.Imaging <a href="https://docs.aspose.com/imaging/java/installation/">Installation instructions</a>. 
