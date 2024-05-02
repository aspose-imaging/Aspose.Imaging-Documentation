---
title: Known Issues
type: docs
weight: 40
url: /ru/python-net/known-issues/
---

## **Python**
- Graphics operations cannot be performed on a BMP which has indexed pixel format.

## Ubuntu Linux

In Ubuntu 22.04, sometimes the following error could be faced
> No useable version of libssl

To resolve, the following steps need to be done
- Download the file libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb  from http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/
- Install it by the command `dpkg -i libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb`

Example:

```
> wget http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
> sudo dpkg -i ./libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
> rm ./libssl1.0-dev_1.0.2n-1ubuntu5.13_amd64.deb
```
