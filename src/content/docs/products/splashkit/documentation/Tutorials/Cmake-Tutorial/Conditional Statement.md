﻿---
title: Conditional Statement
---

In this tutorial we are going to learn how to use the conditional statement in Cmake. This is just
like any other language's if-else statement, let's look an an example:

```cpp
cmake_minimum_required(VERSION 3.5)
set(MAIN "main")

if((${MAIN} STREQUAL  "main")
 project((${MAIN})
 add_executable((${MAIN} "main.cpp")
 message("It is done")
else()
 message("Project not found")
endif()

set_target_properties(MAIN PROPERTIES OUTPUT_NAME "run")
```

In here we are telling Cmake that, if `MAIN` variable is `"main"` if it is then print
`it is done in the console` if not print `project not found`. Run it and it should print out the
message in the console.

Here's all the comparison syntax:

```bash
-   EQUAL
-   LESS
-   LESS_EQUAL
-   GREATER
-   GREATER_EQUAL
-   STREQUAL
-   STRLESS
-   STRLESS_EQUAL
-   STRGREATER
-   STRGREATER_EQUAL
-   VERSION_EQUAL
-   VERSION_LESS
-   VERSION_LESS_EQUAL
-   VERSION_GREATER
-   VERSION_GREATER_EQUAL
-   PATH_EQUAL
-   MATCHES
```
