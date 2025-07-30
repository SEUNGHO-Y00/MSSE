# Expanded C++ Topics - Discussing topics for the final
  - Vectors, Functions, and Multi-file Programs

1. Standard Containers

* std::array Features
  - std::array wraps C-style arrays with additional safety:
    - Same performance as C arrays
    - Knows its own size
    - Provides bounds checking when requested
    - Works with C++ method
   
* Access Methods Compared
  - [] operator
  - .at() Method
 
* When Size Must Be Determined at Runtme
  -  Both C arrays and std::array require compile
 
* std::vector Solves Dynamic Sizing
  - std::vector provides arrays that can change size
 
* Key Vector Methods
  - .size()
  - .push_back(value)
  - .empty()
  - .front()
  - .back
  - .at(index)
 
* std::map Features
  - std::map stores key-value pairs

2. Argument Passing to Functions in C++

* Function Components
  - Return type
  - Function name
  - Parameters
 
* C++'s Default Behavior
  - pass-by-value
 
* Arrays don't follow pass-by-value

* Container Follow Pass-by-Value

* We could use pointers to avoid copying

* C++ provides a better solution: references

* const and & are often used together for large data structures

3. More Functions: Function overloading and returning multiple values

4. C++ Exceptions

5. Organizing Code: Multifile C++ Project

