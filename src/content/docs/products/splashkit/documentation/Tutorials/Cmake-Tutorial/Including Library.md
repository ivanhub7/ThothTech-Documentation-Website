﻿---
title: Including Library
---

Now we covered the fundamental of coding in Cmake, in this tutorial we are learning core feature of
Cmake, which is how to include a library in our project. Before demonstrating of how it works, first
we need to make our own library. In this example we're going to build a custom, library to print
string to our console. first we make a lib folder and create a header file call "print.h"

```cpp
#ifndef PRINT_H
#define  PRINT_H

#include  <iostream>

void  print(const  std::string&  message);

#endif
```

`#ifndef PRINT_H` and `#define  PRINT_H` are telling the compiler that do not include the print.h if
it's already exist. It helps preventing the header from including twice.

then create print.cpp:

```cpp
#include  "print.h"

void  print(const  std::string&  message) {

 std::cout  <<  message  <<  std::endl;
}
```

This is where the print function is, we do not need to include `iostream` since `print.h` already
got it included Now in the CmakeLists.txt

```c
cmake_minimum_required(VERSION 3.5)

set(MAIN "main")
set(LIB_DIRECTORY "./lib")

project(${MAIN})

add_library(print ${LIB_DIRECTORY}/print.cpp)
target_include_directories(print PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/${LIB_DIRECTORY})
add_executable(${MAIN}  "main.cpp")
target_link_libraries(${MAIN} PRIVATE print)

set_target_properties(${MAIN} PROPERTIES OUTPUT_NAME "run")
```

Here we are the `./lib` directory as a variable in-case we need to change it later.

- `add_library(print ${LIB_DIRECTORY}/print.cpp)` we are telling the compiler we are adding this
  library.
- `target_include_directories(print PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/${LIB_DIRECTORY})` we are
  telling where the library is. Note: we can use
  `include_directories(${CMAKE_CURRENT_SOURCE_DIR}/${LIB_DIRECTORY)` if you want, the difference is
  that `include_directories` means that any file you complied are depending the library in that
  exact directory, so if you are working on a big project make sure you know every file needed that
  library.

- `target_link_libraries(${MAIN} PRIVATE print)` which project we are linking the library to Now
  that's done run it, it run print out the message in the console.

## Others

If you curious of other Cmake default keywords like `${CMAKE_CURRENT_SOURCE_DIR}` I would recommend
check the links below as there are a lot of cover:
[Cmake variables](https://cmake.org/cmake/help/latest/manual/cmake-variables.7.html)
