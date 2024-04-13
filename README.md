# Hello, World! - C++

<div align="center">
  <img src="https://img.shields.io/badge/language-C++-blue.svg">
  <img src="https://img.shields.io/badge/standard-C%2B%2B17-blue.svg">
<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/240px-ISO_C%2B%2B_Logo.svg.png" alt="C++ Logo" width="100">
  
</p>
<p align="center">
Logo endorsed by the C++ standards committee
</p>
</div>

## Description

`C++` is a general-purpose programming language created by [Bjarne Stroustrup](https://en.wikipedia.org/wiki/Bjarne_Stroustrup) as an extension of the [C programming language](<https://en.wikipedia.org/wiki/C_(programming_language)>), or "C with Classes". The language has expanded significantly over time, and modern `C++` has object-oriented, generic, and functional features in addition to facilities for low-level memory manipulation.

## The `CMakeLists.txt` File[^1]

For a simple `C++` project (e.g., a "Hello, World!" program), the `CMakeLists.txt`[^1] file is typically very simple.

```txt
.
├── CMakeLists.txt
└── src
    └── hello_world.cpp
```

**_CMakeLists.txt_**[^1]

```cmake
# Set the minimum version of CMake that can be used
cmake_minimum_required(VERSION 3.5)

# Set the project name
project(HelloWorld)

# Add an executable
add_executable(hello_world src/hello_world.cpp)
```

### Running the Program

To run the program, follow these steps:

1. Run `CMake` to configure the project:

```bash
cmake .
```

2. Build the project:

```bash
make
```

4. Run the program:

```bash
./hello_world
```

**To clean the project:**

```bash
make clean-all
```

<!-- Footer -->

[^1]: `CMakeLists.txt` is a simple text file that is used to configure a project that is built using the `CMake` build system. The `CMakeLists.txt` file contains a set of directives and instructions describing the project's source files and targets (executable, library, or both). The `CMakeLists.txt` file must be present in the root directory of the project.
