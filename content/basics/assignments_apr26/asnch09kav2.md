---
title: Asnch09Kav2
date: 2026-05-23
author: Your Name
cell_count: 7
score: 5
---

Chapter 09 – Python Advanced Topics
1. Write a list comprehension that generates a list of squares of all even numbers from 1 to
20.

2. Using a list comprehension with a conditional filter, extract all words longer than 4
characters from the list: ['apple', 'fig', 'banana', 'kiwi', 'mango',
'pear'].
3. Define a lambda function that takes two arguments and returns their product. Assign it to
a variable and demonstrate its usage with an example.
4. Using the map() function along with a lambda, convert a list of temperatures in Celsius
[0, 20, 37, 100] to Fahrenheit.
5. Create a custom iterator class in Python that yields the first n multiples of a given
number. Demonstrate its usage with a for loop.



```python
# num_list = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]

for i in range(1, 20):
    if i%2 == 0:
        sq = (i**2)
        print(sq)
```

    4
    16
    36
    64
    100
    144
    196
    256
    324



```python
fruits = ["apple", "fig", "banana", "kiwi", "mango'","pear"]

newlist = [nfruits for nfruits in fruits 
            if len(nfruits) > 4]
print(newlist)
```

    ['apple', 'banana', "mango'"]



```python
mul = lambda a, b: a * b
print(mul(10, 5))  # Output: 15
```

    50



```python
celsius = [0, 20, 37, 100]
fahrenheit = list(map(lambda c: c * 9/5 + 32, celsius))

print(fahrenheit)
```


```python
a = 1
b = 2






x = iter(celsius)
print(next(x))
print(next(x))
```

    0
    20



```python

```


---
**Score: 5**