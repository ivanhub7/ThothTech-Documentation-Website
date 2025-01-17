﻿---
title: Add Custom Command
---

In this tutorial, we are going to cover how to add custom command to our compiler. This is basically
telling what the compiler should do like copy the file, change directory etc. In this example we
merely going to learn how to move files in a directory:

```c
add_custom_command(
TARGET ${MAIN}
 POST_BUILD
 COMMAND  ${CMAKE_COMMAND} -E copy_directory ${CMAKE_SOURCE_DIR}/lib ${CMAKE_BINARY_DIR}/new_lib
)
```

In this code we are moving the files in the directory to another directory which in this case
`new_lib`. `Targer ${Main}` : This is basically telling Cmake to track the target `POST_BUILD` This
tells the compiler to move after the project is built, here are other keyword you need to know:

```c
PRE_BUILD - run before all other dependencies
PRE_LINK - run after other dependencies
POST_BUILD - run after the target has been built
```

`COMMAND`: This is somewhat like the powershell command you use. To learn the commands, please
reference the link below.
[Cmake Commands](https://cmake.org/cmake/help/latest/manual/cmake.1.html#cmdoption-cmake-E)
