---
title: Functions Asmt
date: 2026-04-18
author: Your Name
cell_count: 17
score: 15
---

```python
def greet():
    return("hello Python")

print(greet())
```

    hello Python



```python
def greet(a):
    print("hello,", a)

greet("python!")
```

    hello, python!



```python
x = lambda y: y ** 2
print(x(6))
```

    36



```python
y = input("enter a value:")


x = lambda y: y ** 2 
print(y)
```

    enter a value: 6


    6



```python
def abc(square):
    print(square**2)

abc(4)

```

    16



```python
def add(a, b):
    print(a+b)

add(4, 5)
```

    9



```python
a = 3

if a % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")


```

    Odd Number



```python
a = 20
b = 10

if a > b:
    print("a is greater")

else:
    print("b is greater")
```

    a is greater



```python
# Factorial

# # def fac(n):
#     return n * fac(n-1)

# fac(2)
```


```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

    120


def factorial(n):
    result = 1
    for i in range(6, n+1):
        result *= i
        return result
print(factorial(10))


```python
def factorial(n):
    result = 1
    for i in range(2, n+1):
        result *= i
    return result
x = print(factorial(5))
print(x)
```

    120
    None



```python
def count_vowels(s: str):
    return sum(1 for char in s if char.lower() in "aeiou")
print(count_vowels("Hello World"))
```

    3



```python
list = (1, 4, 4)
print (sum(list))
```

    9



```python
def sum_list(num: list):
    return (sum(num))

print(sum_list([1,4,5]))

```

    10



```python
def rev(a):
    return a[::-1]

print(rev("Angela"))
```

    alegnA



```python

```


---
**Score: 15**