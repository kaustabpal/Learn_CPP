# Build System

The process of compiling a C++ code is as follows:

1. Source code
2. Pre-processor
3. Compiler
4. Linker
5. Executable

## Source code

The source code is the code written by the programmer. 

## Pre-processor

The source code contains all the header files. The preprocessing step unwraps all the header files and puts them all in a single file along with the user written code. 

The command to do that is: ```clang++ -E main.cpp > main.i```

## Compilation

This step translates the pre-processed code to assembly code. This will also update the ```main.o``` object file. 

The command to do this will be: ```clang++ -S main.i```

## Linking

We link multiple object files and libraries to create an executable. 

The command to do this is: ```clang++ prog1.o main.o -o main```
