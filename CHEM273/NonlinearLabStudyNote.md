# Solving Nonlinear Equations Lab

1. Recursion
* Recursive programming is when a function calls itself
* A recursive function breaks a large problem into smaller version of same

2. Recursive Functions - Example
```python
def countdown(n):
  if(n==1):
    print(n)
  else:
    print(n)
    countdown(n-1)
```
4. Recursion
* Recursive functions have two "cases":
  - The base case, the "end" result where the function is not called
  - The recursive case, where the function calls iteself

5. Recursion example
* factorials
```python
def factorials(n):
  if (n == 0):
    return 1
  else:
    return n * factorials(n - 1)
```
6. Recursion - Practice

