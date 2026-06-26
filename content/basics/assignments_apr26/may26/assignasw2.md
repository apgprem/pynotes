---
title: Assignasw2
date: 2026-06-26
author: Your Name
cell_count: 7
score: 5
---

```python
Python Variable Scope
1 Write a Python program that defines a local variable inside a function and prints it.
Example
def show():
    x = 10
    print(x)
    
2 Write a Python program that creates a global variable and prints it inside a function.
    
3 Write a Python program that shows the difference between a local variable and a global variable with the same name.
Example
x = 100
def test():
    x = 50
    print(x)
    
4 Write a Python program that accesses a global variable inside a function.
5 Write a Python program that modifies a global variable inside a function using the global keyword.
6 Write a Python program that creates two functions and accesses the same global variable from both functions.
7 Write a Python program that demonstrates a local variable not accessible outside the function.
8 Write a Python program that creates a function inside another function and accesses the outer function variable.
Example
def outer():
    x = 10
    def inner():
        print(x)
9 Write a Python program that demonstrates the nonlocal keyword in a nested function.
10 Write a Python program that modifies an enclosing variable using nonlocal.
```


```python
def loclvar():
    a = 10
    print(a)

loclvar()
```

    10



```python
b = 20
def glblvar():
    print(b)
    
glblvar()
```

    20



```python

a=11
def loclvar():
    a = 10
    print(a) # local var

loclvar()
print(a) # global var
```

    10
    11



```python
#  7

def loclvar():
    x = 11
    print("local",x)

loclvar()
print("outside function",x)

```

    local 11



    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[1], line 8
          4     x = 11
          5     print("local",x)
          6 
          7 loclvar()
    ----> 8 print("outside function",x)


    NameError: name 'x' is not defined



```python
def outer():
    x = 10
    def inner():    
        print(x)
    inner()
outer()
```

    10



```python

```


---
**Score: 5**