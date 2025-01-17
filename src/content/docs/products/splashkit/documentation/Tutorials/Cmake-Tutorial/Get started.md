﻿---
title: Getting Started With Sprite Layering In Splashkit - C++
---

Welcome to this CMake tutorial. We'll cover the fundamental features of CMake, a project management
tool used to guide the compilation process for various operating systems. CMake is commonly employed
for tasks like library management and software testing to ensure proper functionality.

## Install Pre-requisites

- Download and Install MSYS in <https://www.msys2.org/>
- prompt these commands:

> pacman -S git --noconfirm --disable-download-timeout bash <(curl -s
> <https://raw.githubusercontent.com/splashkit/skm/master/install-scripts/skm-install.sh>)

- prompt "skm" ensure everything is good to go
- Install compilers:

> pacman --disable-download-timeout -S mingw-w64-{x86_64,i686}-gcc mingw-w64-{i686,x86_64}-gdb

- Install cmake and make:

> pacman -S mingw-w64-x86_64-cmake pacman -S mingw-w64-x86_64-make

### Table of Content

1. [Build your first project](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/2.%20Build%20our%20First%20Cmake.md)
2. [Variables](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/3.%20Variables.md)
3. [Conditional Statement](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/4.%20Conditional%20Statement.md)
4. [Loop Statement](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/5.%20Loop%20statement.md)
5. [Including Library](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/6.%20Including%20Library.md)
6. [Add Custom Command](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/7.%20Add%20Custom%20Command.md)
7. [Cross-platforming](https://github.com/MangoS9/SplashKit-Tutorial/blob/main/Cmake%20Tutorial/7.%20Add%20Custom%20Command.md)

### Additional Information

1. [Build your first project](./2.%20Build%20our%20First%20Cmake.md)
2. [Variables](./3.%20Variables.md)
3. [Conditional Statement](./4.%20Conditional%20Statement.md)
4. [Loop Statement](./5.%20Loop%20statement.md)
5. [Including Library](./6.%20Including%20Library.md)
6. [Add Custom Command](./7.%20Add%20Custom%20Command.md)
7. [Cross-platforming](./8.%20Cross-platforming.md)

### Expected Learning Outcomes

The learning outcome that the reader can expect to have gained after the completion of this tutorial
is to have a basic understanding of Cmake, including the understanding of library management for
different operating system.
