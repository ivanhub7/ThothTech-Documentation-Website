﻿---
title: Cross Platforming
---

In this tutorial, we are covering how to apply conditions depending on different operating system.
It is relatively simple, all you need to do is using the conditional statement and check the special
keyword built in Cmake:

````c
```cmake
if(WIN32)
    # Windows-specific code or configuration
elseif(APPLE)
    # macOS-specific code or configuration
elseif(UNIX)
    # Unix/Linux-specific code or configuration
else()
    message(FATAL_ERROR "Unsupported platform")
endif()
````

That is it!Congrats on learning the basic of Cmake. If you wish further your skill of mastering
Cmake, I recommend going to this website right here:
[Cmake tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/index.html)
