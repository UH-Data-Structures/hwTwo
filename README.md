# hw2, Recursive Notifications. Due date: Friday 10/7

You will create a C++ program that will recursively combine notifications (using doubly linked lists).

The requirements are the same as those of hw1 unless explicitly indicated here.

## Program specification

The main program should be called `coogsive` and the syntax in which it will be tested is as follows:

`./coogsive "input=FILENAME"`

Example of program calls:

`./coogsive "input=uh-gray.1.txt"`

The source code will be compiled as follows:

`g++ -std=c++11 -o coogsive -I ./ *.cpp`


Example of combining notifications from all input files:

    File 1 has notifications 
    A s1 b1
    B s2 b2
    C s3 b3
    D s4 b4

    File 2 has notifications 
    G s5 b5
    H s6 b6
    K s7 b7

    File 3 has notifications 
    M s8 b8
    N s9 b9

    File 4 has notifications 
    Q s10 b10
    R s11 b11
    T s12 b12
    S s13 b13

    The global list would be: 
    A s1 b1
    G s5 b5
    M s8 b8
    Q s10 b10
    B s2 b2
    H s6 b6
    N s9 b9
    R s11 b11
    C s3 b3
    K s7 b7
    T s12 b12
    D s4 b4
    S s13 b13
    
## Requirements

* Must utilize your own linked-lists to do the combining of operations (either within a file, or when combining various files into a single list of notifications). Failure to do so will result in a grade of 2 points (out of 100). That is, using any existing library for linked-lists is not allowed.
* Everything in your code needs to be done via recursion instead of via loops (such as `for` or `while`). Each time that your program uses a `for` or `while` loop (or similar) will have a penalty of 27 points (out of 100).
