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

3. if, else, and elif

```python
for n in range(10)"
  if n%2 == 0: # applies if a condition is true // a logical condition (therefore ==)
    print('even number: ' + str(n))
  else:
    print('odd number: ' + str(n))
```

```python
for n in range(10)"
  if n%2 == 0:
    print('even number: ' + str(n))
  elif n%3 == 0: # elif is not continue other statement
    print('nultiple of 3: ' + str(n))
  elif n%5 == 0:
    print('nultiple of 5: ' + str(n))
  else:
    print('odd number: ' + str(n))
```

4. while

```python
n = 0

while n < 10:
  n += 1
  print(n)
```

5. break, continue, and pass
```python
L = ['a','b','c','d','e']
R = range(10)
T = (-1, ['a','b'], 'this is a string')

for idx, (I, j, k) in enumerate(zip(L,R,T)):
  print(idx, I,j,k)
```

* Checking, if integer N>3 is a prime number. Now we also want the code to print if N is prime too.
```python
N = 40
for n in range(3,N):
  result = N%n

  if result == 0:
    print('not prime')

    break
  else:
    if n < N-1:
      continue
    print('is prime')
```

* For Loops comprehension

```python
from math import
# standard
N = 10
F = [None] * N

for n in range(N):
  F[n] = factorial(n)
# comprehension
FC = [factorial(n) for n in range(N)]
```

```python
NT = 'ACGT'
Code = [[1,0,0,0],
        [0,1,0,0],
        [0,0,1,0],
        [0,0,0,1]]
#standard
Dict = {}

for key, value in zip(NT, Code):
  Dict[key] = value
#comprehension
DictC = {key: value  for key, value in zip(NT, Code)}
```

