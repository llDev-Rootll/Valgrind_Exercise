
# C++ Boilerplate
[![Build Status](https://travis-ci.org/dpiet/cpp-boilerplate.svg?branch=master)](https://travis-ci.org/dpiet/cpp-boilerplate)
[![Coverage Status](https://coveralls.io/repos/github/dpiet/cpp-boilerplate/badge.svg?branch=master)](https://coveralls.io/github/dpiet/cpp-boilerplate?branch=master)
---

## Overview

Simple starter C++ project with:

- cmake
- googletest

## Standard install via command-line
```
git clone --recursive https://github.com/dpiet/cpp-boilerplate
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app
```

## Building for code coverage 
```
sudo apt-get install lcov
cmake -D COVERAGE=ON -D CMAKE_BUILD_TYPE=Debug ../
make
make code_coverage
```
This generates a index.html page in the build/coverage sub-directory that can be viewed locally in a web browser.

## Valgrind

The initial valgrind output can be seen [here](https://github.com/llDev-Rootll/Valgrind_Exercise/blob/valgrind_exercise/initial_valgrind_output.txt).
The final valgrind out can be seen [here](https://github.com/llDev-Rootll/Valgrind_Exercise/blob/valgrind_exercise/final_valgrind_output.txt).

 - Misuse of uninitialized value fixed by initializing boolean variable in main.cpp
 - Memory leak fixed by deleting vector of pointers in AnalogSensor.cpp

Screenshot of KCachegrind can be seen [here](https://github.com/llDev-Rootll/Valgrind_Exercise/blob/valgrind_exercise/KCachegrind.png).
