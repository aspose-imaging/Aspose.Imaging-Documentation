---
title: System requirements
type: docs
weight: 90
url: /python-net/system-requirements/
description: You can use Python Image Processing Library API to develop applications in any development environment that targets the .NET platform.
---

### **Supported Operating Systems:**
Aspose.Imaging for Python via .NET supports Windows 32/64-bit, Linux 64-bit, MacOS x64/arm64 operating systems where Python 3.5 or later is installed.

<table>  
	<tr>
			<td style="font-weight: bold; width:400px">Operating System</td>
			<td style="font-weight: bold; width:400px">Versions</td>
		</tr>
  <tr>
			<td>Microsoft Windows</td>
			<td><ul><li>Windows 2003 Server (x64)</li><li>Windows 2008 Server (x64)</li><li>Windows 2012 Server (x64)</li><li>Windows 2012 R2 Server (x64)</li><li>Windows 2016 Server (x64)</li><li>Windows 2019 Server (x64)</li><li>Windows XP (x64)</li><li>Windows Vista (x64)</li><li>Windows 7 (x64)</li><li>Windows 8, 8.1 (x64)</li><li>Windows 10 (x64)</li><li>Windows 11 (x64)</li></ul></td>
		</tr>
  <tr>
			<td>Linux</td>
			<td><ul><li>Ubuntu</li><li>OpenSUSE</li><li>CentOS</li><li>and others</li></ul></td>
		</tr>
		<tr>
			<td>MacOS</td>
			<td><ul><li>MacOS x64 (Intel)</li><li>MacOS Arm64 (M1/M2/M3)</li></ul></td>
		</tr>
</table>

{{% alert color="primary" %}} 

Aspose.Imaging works for only x64 versions of the above listed operating systems.

{{% /alert %}}

### **System Requirements for Target Linux Platforms**
- GNU libc >= 2.17<br/>
  To get to know your version, you could execute a command<br/>
  `ldd --version`
- GCC-6 runtime libraries (or later).
- libgdiplus: an Open Source implementation of the GDI+ API.
- Dependencies of .NET Core Runtime. Installing .NET Core Runtime itself is NOT required.
- For Python 3.5-3.7: The pymalloc build of Python is needed. The --with-pymalloc Python build option is enabled by default. Typically, the pymalloc build of Python is marked with m suffix in the filename.
- libpython shared Python library. The --enable-shared Python build option is disabled by default, some Python distributions do not contain the libpython shared library. For some linux platforms, the libpython shared library can be installed using the package manager, for example: sudo apt-get install libpython3.7. The common issue is that libpython library is installed in a different location than the standard system location for shared libraries. The issue can be fixed by using the Python build options to set alternate library paths when compiling Python, or fixed by creating a symbolic link to the libpython library file in the system standard location for shared libraries. Typically, the libpython shared library file name is libpythonX.Ym.so.1.0 for Python 3.5-3.7, or libpythonX.Y.so.1.0 for Python 3.8 or later (for example: libpython3.7m.so.1.0, libpython3.9.so.1.0).

