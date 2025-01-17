﻿---
title: Variables
---

In this tutorial we are going to cover how to declare variables in Cmake. Just like other
programming, Cmake has variable for:

```bash
strings: "I like cheese"
integer: 2,3,4,5
float: 2.334
boolean: TRUE or FALSE
```

Luckily for us, unlike C++ we don't need to declare the datatype. Let's look at an example:

```c
cmake_minimum_required(VERSION "3.5")
set(MAIN "main")

project(${MAIN})
add_executable(${MAIN}"main.cpp")

set_target_properties(${MAIN} PROPERTIES OUTPUT_NAME run)
```

`set(MAIN "main")` In here we are telling Cmake that the variable `MAIN` has the string call
`'main'`. Then we replace the string in the code with the variable name instead. Run it by prompting
and it should output the same as the last tutorial.

Note: It is optional to use ${..} in Cmake to reference a variable, like instead of

```c
project(${MAIN})
add_executable(${MAIN} "main.cpp")
```

we can use

```c
project(MAIN)
add_executable(MAIN "main.cpp")
```

In big project, ${..} is very useful to improve readability of the code. It tells the user that it
is a "declared variable". Again it is optional, but it is a good practice if you are working in a
team of a project.

Note: If you wish to tell the Cmake to ignore a code or just put a comment to remind yourself, just
put '#' at the front and Cmake wont run that code. example:

```c
# project(MAIN)
```
