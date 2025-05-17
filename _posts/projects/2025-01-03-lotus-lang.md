---
layout: project-lotus
title:  "Lotus"
teaser: "A statically-typed procedural programming language with an interpreter built in C++."
tags:
    - post format
categories:
    - projects
image:
    thumb: projects/lotus-thumb.png
    title: projects/lotus-thumb.png
show_meta: false
gallery:
github: https://github.com/Multipixels/lotus-lang
header: false
---

Lotus is a programming language I developed to explore the principles of statically-typed procedural languages, test-driven development, and software testing. With Lotus, you can write programs using familiar constructs like collections, dictionaries, and control structures, all parsed and interpreted through an interpreter written in C++.

### Built With

* C++
* [CMake](https://cmake.org/)
* [Emscripten](https://emscripten.org/)
* [Google Test](https://google.github.io/googletest/)
* [Visual Studio](https://visualstudio.microsoft.com/)

### Prerequisites

Ensure you have the following installed:

* A C++ compiler
* CMake

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Multipixels/lotus-lang.git
   ```
2. Navigate to the project's root directory:
   ```sh
   cd lotus-lang
   ```
3. Generate a new directory `out` and navigate to it:
   ```sh
   mkdir out
   cd out
   ```
4. Run CMake:  
   For just the Lotus interpreter, run
   ```sh
   cmake ..
   ```
   For the Lotus interpreter and test suites, run
   ```sh
   cmake .. CMAKE_BUILD_TYPE=Debug
   ```
   
5. Compile the project.  
   i. (Windows) Open solution `out\LotusLang.sln` in Visual Studio and build.  
   ii. (Mac/Linux) Run `make`

6. (Optional, Windows only) Compile the project for the web w/ Emscripten. Requires Emscripten installed and setup.
   ```
   mkdir out
   cd out
   mkdir build-wasm
   cd build-wasm
   
   call emcmake cmake ../..  -D DCMAKE_SYSTEM_NAME=Emscripten
   
   cmake --build . --target LotusLangWeb
   ```

### Usage

#### CLI Interpreter

To open up the interpreter in your CLI, simply run the binary.

- (Windows):
```
.\LotusLang.exe
```

- (Mac/Linux):
```sh
./LotusLang
```

#### Interpret Lotus Code from Files

Write Lotus programs in `.lotus` files and run them through the interpreter. Here's an example program:

```
-> Find the sum of the values in a collection
integer sum = 0;
collection<integer> myCollection = [2, 4, 6];

iterate(value : myCollection) {
  sum += value;
}

log(sum);
```

Run the program

- Windows:
```
.\LotusLang.exe example.lotus
```
- Mac/Linux:
```sh
./LotusLang example.lotus
```

### Features

- **Statically-Typed Variables**: Includes primitive types like `boolean`, `integer`, `float`, `character`, and `string`.
- **Collections and Dictionaries**: Flexible and easy-to-use data structures.
- **Functions**: Define reusable blocks of code with return types and parameters.
- **Control Structures**: Use logic and loop structures, like `if-else`, `while`, `for`, and more.
- **Built-in Functions**: Log messages to the console, modify collection contents, and more.
