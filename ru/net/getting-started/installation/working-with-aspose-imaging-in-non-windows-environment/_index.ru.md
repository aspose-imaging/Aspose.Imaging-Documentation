---
title: Working with Aspose.Imaging .NET Core DLLs in non Windows environment
type: docs
weight: 50
url: /ru/net/installation/working-with-aspose-imaging-in-non-windows-environment/
description: This article describes how to work with Aspose.Imaging dlls in non Windows environment.
---

## **Working with Aspose.Imaging .NET Core DLLs in Linux like operating systems**
Aspose.Imaging is cross-platform library that supports popular platforms, among which is Linux based systems. To succesfully run Aspose.Imaging on such platforms users need to perform some additional steps to install some needed dependencies.

## **Working with .NET Standard2.0, .NET Core 2.0, .NET Core 3.1, .NET5, .NET6 dlls**

As Aspose.Imaging for .NET provides .NET Standard 2.0 (.NET Core 2.0, .NET Core 3.1 and .NET5) and .NET6 support, it can be used in Core Applications running in Linux like operating systems. We are constantly working over improving the .NET Core support in our API. However, there are some following operations which we recommend our customers to perform, in order to get better results while using features of Aspose.Imaging for .NET.

Please install:
1. libgdiplus package
1. libc6-dev package
1. package with Microsoft compatible fonts: ttf-mscorefonts-installer (e.g. *sudo apt-get install ttf-mscorefonts-installer*)
1. package with other fonts: *apt-get update && apt-get install -y fontconfig fonts-wqy-zenhei*

### **How to install libgdiplus package on Ubuntu Linux**
To install libgdiplus package you can follow instruction:

sudo apt install gnupg ca-certificates

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF

echo "deb https://download.mono-project.com/repo/ubuntu stable-bionic main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list

sudo apt update

sudo apt install libgdiplus

More information you can get at https://www.mono-project.com/download/stable/#download-lin

## **Working with .NET7 dlls**
Version of .NET7 dlls for Aspose.Imaging uses alternative graphics engine - [Aspose.Drawing](https://products.aspose.com/drawing/ru/net/) instead of System.Drawng.Common/GDI+, so user does not require to use any additional graphics engine to work with library. There are some following operations which we recommend our customers to perform, in order to get better results while using features of Aspose.Imaging for .NET.
Please install:
1. Default fonts: *sudo apt-get update sudo apt-get install fonts-freefont-ttf*
1. Microsoft fonts (if necessary): *sudo apt-get install ttf-mscorefonts-installer*
1. Other fonts: *apt-get update && apt-get install -y fontconfig fonts-wqy-zenhei*

