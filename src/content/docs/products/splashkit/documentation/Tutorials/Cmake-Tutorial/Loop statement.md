﻿---
title: Loop statement
---

In this tutorial we are going to cover the different loop statement in Cmake. Unfortunately, Cmake
only has 1 type of loop which is `foreach()` loop, but this is all we needed for this language.

```c
cmake_minimum_required(VERSION 3.5)

set(MAIN "main"  "main2"  "main3")

# if(MAIN STREQUAL "main")
# project(MAIN)
# add_executable(MAIN "main.cpp")
# message("It is done")
# else()
# message("Project not found")
# endif()

foreach(main ${MAIN})
 project(${main})
 add_executable(${main}  "${main}.cpp")
 message("${main}: It is done")
endforeach()

# set_target_properties(MAIN PROPERTIES OUTPUT_NAME "run")
```

In this example we are going output 3 main files using loop. `set(MAIN "main"  "main2"  "main3")`
this is what you call a list, which stores multiple different value in a variable. Run it and it
will output 3 main files as exe
