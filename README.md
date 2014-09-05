SFU-CMPT225
===========

2014 Fall - Data Structure and Algorithm

Office: after class on Monday and Friday. 

### Reverse Polish Notation (RPN)

You cannot get the stack on the bottom untill you remove everything on the top.

Stack is an abstract data types: hiding the details of implementation from the user. 

Example of Stacks

1. Mutators
2. Accessors
3. Constructors
4. Other

```
MyStack st1(5);

MyStack st2(3);

st1.Push(4); //st1 only contains 4

st2.Push(223); // st2 only contains 223

```

```
int r = 3; // local variable integer
double area = CircleArea(r); // 

double CircleArea(double radius) {
  double pi = 3.1415;
  double sq_r = Square(radius);
  return sq_r *pi;
}

double Square(double x) {
  
}

```

### Stack Implementation
Stack implementation
``` 
/*
  User is only presented with int x, 
  the implementation of the function could be changed.
  As far as user is concerned, they just need to call this function.
*/
void push(int) 
int pop()

```

Top of the stack is where the operation happening.

### Arrays in C++ 

The []s should contain the size of the array which must be a constant or literal integer.

```
int age[100];
const int DAYS = 365;
double temperatures[DAYS];
```

```
int arr_size = 5;
int some_ints[5];

some_int[0] = 410;
some_int[1] = 223;
some_int[4] = 22;

for(int i = 0; i < arr_size; i++) {
  some_int[i] = i+45;
}

int fib[] = {0, 4, 5, 23, 64, 53, 34, 9};
```

Array itself is not a class, so it doesn't have size method.
Size is not a inherent feature of Array.


``` 
int arr1[4];
int arr2[3];

arr1 = arr2; // can't do this!
arr1 = {1, 3, 5, 7};

//Array elements can be assigned values
for(int i = 0; i < 4; i++) {
  arr1[i] = arr2[i];
}

```

### Memory in C++

A pointer is a integer address that is stored in the stack memory.



```
int* p_arr = new int[100];
for (int i = 0; i < 100; ++i) {
  p_arr[i] = i+1;
}

delete[] p_arr; //release memory
p_arr = new int[10000000];

```

### Pointer

```

#include <iostream>
using namespace std;

int main()
{
  int originArray[5];
  
  originArray[0] = 11;
  originArray[1] = 22;
  originArray[2] = 33;
  originArray[3] = 44;
  originArray[4] = 55;
  
  int* dynamicArray = new int[5];
  
  *dynamicArray[1] = 11;
  
  
  return 0;  
}








