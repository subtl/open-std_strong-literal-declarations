Abstract
========
This paper introduces a couple new syntaxs to enable C/C++ developers to provide strict enum and literal function parameters, and variables. Thus potentially catching run-time errors at compile-time.

Motivation
==========
To be written.

Introduction
============
Classic way

```c++
enum Options : int {
  OPT_ONE,
  OPT_TWO,
  OPT_THREE
  // etc.
};

void set_option(Options);

// ...

set_option(Options::OPT_ONE);
```

New Way

```C++
enum Options : int {
  OPT_ONE,
  OPT_TWO,
  OPT_THREE
  // etc.
};

void set_option([Options]);

// ...

set_option([OPT_ONE]);
```
