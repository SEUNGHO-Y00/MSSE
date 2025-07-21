# Deeper C++ Exploration

1. C++ Vocabulary: Variable Definition and Declaration

* Declaration
  - defines the variable type and name

* Definition
  - Gives the variable a value 

2. C++ Control Structures: Loops

* for loop
  - for (int i = 0; i < 10; i++) //Initialization|Test|Increment
 
* while loop
  - while (i<10) { i++; }
  - continue: stops execution the body and starts a new iteration from the beginning of the body
  - break: exits the loop immediately

3. C++ Addresses and Pointers

* Pointers "point to" a variable whose address they store
* Every variable has a memory address where its data is stored
* You can access that address using the & operator (address-of)
* A pointer is a variable that stores a memory address
* You can declare a pointer using * (type of pointer sould match type its pointing to)
* You "dereference" a pointer using * to access or modify the value it points to
* You can reassign a pointer to point to a different variable using assignment and &

4. Data Types: Arrays and Vectors

* C style arrays do not include bounds checking.
