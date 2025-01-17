---
title: Building the SplashKit Core Library with CMake
---

## Introduction

In this tutorial we are going the cover how to build splashkit core library in our project using
Cmake. Splashkit-core already had a pre-made `CmakeLists.txt` file in
`splashkit-core\projects\cmake`. Feel free to explore and tinker the setting over there.

### Build and test

- fork and clone splashkit:

> git clone --recursive -j2 <https://github.com/>username/splashkit-core.git

[I have made a script that automatically run everything below, check "issue troubleshot and other
things (On windows)"]

- Change directory and run cmake:

> cd projects/cmake cmake -G "Unix Makefiles" .

- prompt "make" to build the test file

make

- Change directory to bin

> cd ../../bin

- run the test and enjoy

> ./sktest

### Make changes or addition to the test

If you like to add feature or make changes to the test file feel free to hop in
"splashkit-core\coresdk\src\test" and make changes there. For the menu changes (assume that is what
you are looking for ), you can either you can add a new cpp file, add the header in "test_main.h"
then change the menu in "test_main.cpp" or change the "test_main.cpp" code in your hearts desire
then rerun the cmake and make above.

### issue troubleshot and other things (On windows)

- If you encounter an error "#include # cstdint>" in "networking.h" just hop into
  "splashkit-core\coresdk\src\coresdk"

open up "networking.h" and include the cstdint library there

- If you encounter an error for "**_darwin_check_fd_set_overflow" just go to the "CMakeLists.txt"
  and comment out all of the "target_link_options(skunit_tests PUBLIC
  "LINKER:-U,_**darwin_check_fd_set_overflow")". This is a linker for MacOS, so for us windows it is
  not a necessity

- Incase your terminal requires you to change the require minimum version of cmake, just change 3.2
  to 3.5 in the Cmakelist file

- I have made a script file where it runs cmake, make and test automatically. Copy it to the
  "splashit-core" folder and run "./run.sh" using MSYS2 Mingw64 (You welcome :3).
