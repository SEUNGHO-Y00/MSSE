# Functions

1. lambda
* recall loops(comprehension)
* What if we want to encode an entire sequence say 'ACGGTCCGACCT'?
```python
NT = 'ACGT'
Code = [[1,0,0,0],
        [0,1,0,0],
        [0,0,1,0],
        [0,0,0,1]]

S = 'ACGGTCCGACCT'
L = []

for s in S:
  L += [Dict[s]]
```
* benchmarking the loop:
```python
import time

t1 = time.monotonic()

for i in range(10000):
  L = []
  for s in S:
    L += [Dict[s]]

t2 = time.monotonic()
dt = t2 - t1

print("Total runtime: " + str(dt) + ' seconds')
```
* alternative:lambda
```python
Encode = lamda Seq: [Dict[s] for s in Sq]
Encode(S)
```
  - Encode = lamda => defining a function, we name Encode using the keyword lambda
  - Seq: => the input argument (name is arbitrary)
  - [Dict[s] for s in Sq] => defines the sequence of commands the function has to execute
* lambda
  - faster(factor of 2)
  - has to be defined only once
  - named "anonymous function" (not stored in an extra file)

2. map
* multiple sequences
```python
S1 = 'ACGGTCCGACCT
S2 = TTCAGGT
S3 = ATCGGCAATCTGCTTA
S4 = CGTCCGTA

Encode = lambda Seq: [Dict[s] for s in Seq]

S = [S1, S2, S3, S4] # a more efficient way is using map

L = list(map(Encode, S))
```
* complete loop
```python
for i in range(100000):
  for s in S:
    L = []
    for nt in s:
      L += [Dict[nt]]
```
* lambda/map
```python
for i in range(100000):
  L = list(map(Encode, S))
```

3. def
* actual functions/methods in python

```python
def My_fun1(a,b):
  res = a + b
  return(res)
```
def => keyword def detines function
My_fun1 => name of the function
(a,b) => mandatory input arguments
res = a + b => sequence of commands the function has to execute
return(res) => return statement for output

* what can go wrong:
  - too many input arguments
  - too few input arguments
  - confusing calling the function vs saving the function as a new variable
  - when output is not stored in a new variable -> generates output in console
  - calling more output variables then provided by function
  - generating multiple outputs

4. *args and **kwargs
* defualt arguments -> specific value unless stated otherwise
```python
def My_fun2(a,b = 2):
  res1 = a + b
  res2 = a * b
  res3 = a**b
  return res1, res2, res3
```

* optional *args arguments -> when needed for specific settings
```python
def My_fun2(a,b = 2, *power):
  if power:
    print(type(power))
  res1 = a + b
  res2 = a * b
  res3 = a**b
  return res1, res2, res3
```

* why is it a tuple?
  - We switch to a better example:
```python
def BuildSentences(*words):
  Sentence = ''
  for w in words:
    Sentence += ' ' + w
    print(Sentence)
```

* optional keyword **kwargs arguments
  - Let us first check the type:
```python
def Groceries(**items):
  print(items)
```
  - Type will be dictionary
 
* Why is it a dictionary?

