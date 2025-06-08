# Control Structures

1. General Idea and structure
often(not always): iterating over an object

```python
L = ['a', 'b', 'c', 'd', 'e']

for i in L:

  print(i)
```
  - i = free index variable

2. For loops and comprehension

```python
for i in L:

  print(i)
```
  - L = iterable object: list, array, range, data frame, etc

* iterating over the content and index of an object
```python
for i, j in enumerate(L):

  print(str(i) + str(j))
```

* Iterating over two objects simultaneously
```python
R = range(0,10,2)
for i, j in zip(R,L):

  print(str(i) +str(j))
```

* iterating over two objects simultaneously and over indices and content
```python
for I, (j, k) in enumerate(zip(R, L)):

  print(str(i) + str(j) + k)
```

* The more pythonic way is using comprehension
```python
from math import *
N = 10
Factorial = [None]*N

for n in range(N):
  Factorial[n] = factorial(n)
```

* Comprehension
```python
Factorial = [factorial(n) for n in range(N)]
```

* The more pythonic way is using comprehension
```python
NT = 'ACGT'
Code = [[1,0,0,0]
        [0,1,0,0]
        [0,0,1,0]
        [0,0,0,1]]
Dict = {}

for code, nt in zip(Code, NT):
  Dict[nt] = code
```

3. if,else and elif


4. while

5. break, continue and pass

