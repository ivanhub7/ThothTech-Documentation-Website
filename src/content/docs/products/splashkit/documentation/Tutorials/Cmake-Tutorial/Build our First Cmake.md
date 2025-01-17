﻿---
title: Build your first Cmake
---

- Create a simple "cpp" that prints Hello world:

```cpp
#include  <iostream>
using  namespace  std;

int  main(){

cout  <<  "Hello World!"  <<  endl;
return  0;
}
```

- In the same directory, create a special txt file call "CmakeLists.txt"
- open up the file and prompt these code in:

```cpp
cmake_minimum_required(VERSION 3.5)

project("main")
add_executable("main"  "main.cpp")

set_target_properties("main" PROPERTIES OUTPUT_NAME "run")
```

`make_minimum_required(VERSION 3.5)` tell cmake the version required `project("main")` name of the
project "can be anything you like" `add_execuration()` add an executatable for our code, currently
support these file extension:

```bash
-   .c
-   .C
-   .c++
-   .cc
-   .cpp
-   .cxx
-   .cu
-   .mpp
-   .m
-   .M
-   .mm
-   .ixx
-   .cppm
-   .h
-   .hh
-   .h++
-   .hm
-   .hpp
-   .hxx
-   .in
-   .txx
-   .f
-   .F
-   .for
-   .f77
-   .f90
-   .f95
-   .f03
-   .hip
-   .ispc
```

`set_target_properties("main" PROPERTIES OUTPUT_NAME "run")` tells the compiler what name should the
output file be, for this instance we tell the compiler to output the file as name `run`.

- In the MSYS terminal run `cmake -G "Unix Makefiles .` This will generate multiple files. You do
  not need to worry about what those file do.
- Now run `make`, it will output an exe file with your desired file name
- Congrats you have made you first project with Cmake

## Others

There are a lot of thing can be added in `set_target_property()` for those information, it can be
found here:
[Cmake set_target_property](https://cmake.org/cmake/help/v3.0/command/set_target_properties.html)
