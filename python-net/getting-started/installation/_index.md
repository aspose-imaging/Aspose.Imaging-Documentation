---
title: Installation
type: docs
weight: 50
url: /python-net/installation/
keywords: "Download Aspose.Imaging, Install Aspose.Imaging, Aspose.Imaging Installation, Windows, Python"
description: Install Aspose.Imaging for Python via .NET in Windows or Linux
---

The Aspose.Imaging for Python via .NET package comes with the .NET libraries it needs, so a separate .NET installation is not required. However, depending on your platform, you may have to install specific dependencies for .NET and meet certain requirements.

## **Windows**

**System Requirements**

Check and confirm that your machine's specifications meet or better the [system requirements](/imaging/python-net/system-requirements/).

### **Install Aspose.Imaging**

`pip` is the easiest way to download and install [Aspose.Imaging for Python via .NET](https://pypi.org/project/aspose-imaging-python-net/) on Windows devices or `pip3` in Linux.

To install Aspose.Imaging, run this command:  
`pip install aspose-imaging-python-net`
or
`pip3 install aspose-imaging-python-net`

## **Working in Non-Windows Environment**
As Aspose.Imaging for Python via .NET based on .NET Core platform, so it can be used in Core Applications running in Linux like operating systems. We are constantly working over improving the .NET Core support in our API. However, there are some following operations which we recommend our customers to perform, in order to get better results while using features of Aspose.Imaging for Python via .NET:

**How to check**

1. The version of GLIBC
Please execute
```
ldd --version
```
Output
> .....
> ldd (GNU libc) 2.17
> .....
*The version of GLIBC must be >= 2.17*

2. The version of dotnet platform
Please execute
```
dotnet --list-runtimes
```
Output
> ....
> Microsoft.NETCore.App 6.0.xxx [/usr/share/dotnet/shared/Microsoft.NETCore.App]
> ....

*The version of NETCore.App must be >= 6.0*

If the `dotnet` command is not found, you need to install dotnet-sdk-6.0 package.


### Ubuntu Linux
```
sudo apt-get install -y libssl1.1 wget python3 python3-pip
wget https://packages.microsoft.com/config/ubuntu/<your version>/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb && rm packages-microsoft-prod.deb
sudo apt-get update
sudo apt-get install -y dotnet-sdk-6.0
sudo apt-get install -y libfontconfig1 xfonts-utils
sudo apt-get install -y ttf-mscorefonts-installer
pip3 install wheel
pip3 install aspose-imaging-python-net
```

**Known issue**

In Ubuntu 22.04, sometimes the following error could be faced
> No useable version of libssl

To resolve, the following steps need to be done
- Download the file libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb  from http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/
- Install it by the command `dpkg -i libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb`

Example:

```
wget http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
sudo dpkg -i ./libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
rm ./libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
```


### CentOS 7
```
rpm -Uvh https://packages.microsoft.com/config/centos/7/packages-microsoft-prod.rpm
yum update -y
yum install -y python3.8 python3-pip dotnet-sdk-6.0
yum install -y epel-release
yum groupinstall -y "fonts"
pip3 install wheel
pip3 install aspose-imaging-python-net
```
