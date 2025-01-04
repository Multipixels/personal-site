---
layout: project-screenshots
title:  "Lotus"
teaser: "A statically-typed procedural programming language with an interpreter built in C++."
tags:
    - post format
categories:
    - projects
image:
    thumb: projects/lotus-thumb.png
    image: projects/lotus-thumb.png
show_meta: false
gallery:
github: https://github.com/Multipixels/lotus-lang
header: no
---

Lotus is a programming language I developed to explore the principles of statically-typed procedural languages, test-driven development, and software testing. With Lotus, you can write programs using familiar constructs like collections, dictionaries, and control structures, all parsed and interpreted through an interpreter written in C++.

### Built With

* C++
* [Google Test](https://google.github.io/googletest/)
* [Visual Studio](https://visualstudio.microsoft.com/)

### Prerequisites

Ensure you have the following installed:

* A C++ compiler
* [Visual Studio](https://visualstudio.microsoft.com/)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Multipixels/lotus-lang.git
   ```
2. Navigate to the project's src directory:
   ```sh
   cd lotus-lang/src
   ```
3. Open the `lotus-lang.sln` file in Visual Studio.
4. Build and run the `lotus-interpreter-tests` tests.
5. Build the `lotus-interpreter` project.

### Usage

Write Lotus programs in `.lotus` files and run them through the interpreter. Here's an example program:

```
-- Find the sum of the values in a collection
integer sum = 0;
collection<integer> myCollection = [2, 4, 6];

iterate(value : myCollection) {
  sum = sum + myCollection;
}

log(sum);
```

Run the program:
```sh
./lotus-interpreter example.lotus
```

### Features

- **Statically-Typed Variables**: Includes primitive types like `boolean`, `integer`, `float`, `character`, and `string`.
- **Collections and Dictionaries**: Flexible and easy-to-use data structures.
- **Functions**: Define reusable blocks of code with return types and parameters.
- **Control Structures**: Use `if-else`, `while`, `for`, and more.
- **Built-in Functions**: Log messages, calculate lengths, and more.

### Roadmap

- [X] &ensp; Basic Syntax and Grammar
- [X] &ensp; Functions
- [X] &ensp; Control Structures
- [X] &ensp; Collections
- [ ] &ensp; Dictionaries
- [ ] &ensp; Strings
- [ ] &ensp; Error Reporting Improvements
- [ ] &ensp; Garbage Collection
- [ ] &ensp; Standard Library Functions