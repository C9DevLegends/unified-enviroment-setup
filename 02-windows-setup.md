# Windows Setup

Greetings, Windows users! Your operating system has a unique lineage, 
tracing back to MS-DOS and Windows NT. In contrast, macOS and Linux 
follow a "Unix" style operating system. [@C9DevLegends](https://github.com/C9DevLegends), we will 
be utilizing the Unix command line to ensure uniformity in tools 
and programs across the project. As Windows lacks a built-in 
Unix-style system, we'll employ a Microsoft Technology 
add-on known as "Windows Subsystem for Linux" (WSL).


## WSL Overview

Windows Subsystem for Linux (WSL) functions as a virtual Linux computer running on your PC. 
It provides the same tools and command line utilities as your macOS and Linux-using teammate.

To install WSL, your Windows 10 version must meet specific criteria:

> For x64 systems: Version 1903 or higher, with Build 18362 or higher.

If your system doesn't meet these requirements, or if you encounter difficulties updating, please reach out to Your team leader.


## Installing WSL 2

While future Windows versions will have an automated WSL installer, 
the current process requires manual installation. 
Follow the instructions in the 
[Windows Subsystem for Linux Installation Guide for Windows 10] 
to install WSL 2 and Ubuntu Linux.

## Tips for WSL Usage

- When prompted to open a Terminal, launch the Ubuntu terminal.
- Store code files in your Ubuntu home directory for improved performance and stability.
- To access Ubuntu home directory files in Windows Explorer, type `Windows + R`, then enter `\\wsl$\home\<your-user>`.
- Access your Windows hard drive from Ubuntu using the path `/mnt/c` within the Ubuntu virtual machine.
- To restart the Ubuntu virtual machine, open a Powershell window and execute:

```shell
wsl --shutdown
```

Upon reopening the Ubuntu terminal, the virtual machine will restart.
## Install Additional Tools

Now that WSL is set up, proceed to install the following tools in order:

1. [Google Chrome]
2. [Visual Studio Code]
3. [Node.JS]
4. [Python]
5. [Docker]

Note: Even if you have some of the listed software installed, carefully read through all instructions. Updates or configuration changes may be necessary.
