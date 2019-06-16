# CppND-Garbage-Collector
The final project for this Memory Management course is to implement your own version of a smart pointer. You can think of this as implementing your own garbage collector, to use a concept from other programming languages. Building this project will help you understand both how to work with pointers and references, and also why smart pointers are so important to modern C++ programming. Complete the implementations and verify that your implementation does not have any memory leaks!

## Project TODO List:
- Complete `Pointer` constructor
- Complete `Pointer` `operator==`
- Complete `Pointer` destructor
- Complete `PtrDetails` class

## Smart Pointer Implementation
The Smart Pointer implementation makes use of three main classes:
* Pointer -> is the class used as Smart Pointer. It aims to reproduce a basic pointer for generic types but improving it by including some features of memory management which will ensure the deallocation of the pointed memory when the Pointer goes out of scope. The Pointer can make reference to a single generic type element as well as an array of such elements.
* Iter -> is a class used to move through the array of element pointed by the Pointer class when this exists.
* PtrDetails -> is a class consisting of an element of the garbage collector of the Pointer.
