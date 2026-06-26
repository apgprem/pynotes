---
title: Assignasw1
date: 2026-06-26
author: Your Name
cell_count: 11
score: 10
---

Python Functions
1 Write a Python function that prints "Hello, Python!" when called.
Example
def greet():
    print("Hello")
2 Write a Python function that takes a number as input and prints its square.
3 Write a Python function that takes two numbers and returns their sum.
Example
def add(a, b):
    return a + b
4 Write a Python function that checks whether a number is even or odd.
5 Write a Python function that returns the largest of two numbers.
6 Write a Python function that calculates the factorial of a number. - Pending
7 Write a Python function that counts the number of vowels in a string. - pending
8 Write a Python function that returns the length of a list.
Example
def list_length(lst):
    return len(lst)
9 Write a Python function that returns the sum of all elements in a list.
10 Write a Python function that takes a string and returns the reversed string.


```python
def greet():
    print("Hello")

greet()
```

    Hello



```python
def greet(a):
    print("the sq value is", a ** 2)
greet(2)
```

    the sq value is 4



```python
def greet(a, b):
    print("sum of a numbers:", a+b)

greet(2,5)
```

    sum of a numbers: 7



```python
def greet(a):
    if a%2 == 0:
        print("even number")
    else:
        print("odd number")
greet(3)
```

    odd number



```python
def greet(a, b):
    if a>b:
        print(a , "is greater")
    else:
        print(b, "is greater")

greet(7,5)
```

    7 is greater



```python

```


```python
list = [1, 4, 4]
print(len(list))


```

    3



```python
list = [1, 4, 4]
print (sum(list))
```

    9



```python
str = "hello"
print(str[::-1])
```

    olleh



```python

```


---
**Score: 10**