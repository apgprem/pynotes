---
title: Assign4
date: 2026-05-25
author: Your Name
cell_count: 8
score: 5
---

Assignment 4: Number Analyzer with Loops and Comprehension
Topics covered: Iteration, list comprehension, sort, reverse, membership
Task: Given a list of numbers, perform analysis using loops and comprehensions.
pythonnumbers = [12, 7, 25, 3, 18, 9, 30, 14, 6, 21]

Use a for loop to print each number along with whether it is even or odd.
Use a list comprehension to create a new list squared containing the square of each number.
Use a list comprehension with a condition to create evens_only containing only even numbers from numbers.
Sort numbers in ascending order, then reverse it to get descending order. Print both.
Check whether 100 is in the list — if not, print "100 is missing".

Expected list comprehension example:
pythonevens_only = [n for n in numbers if n % 2 == 0]


```python
pythonnumbers = [12, 7, 25, 3, 18, 9, 30, 14, 6, 21]

for i in pythonnumbers:
    if i%2 == 0:
        print("Even Number", i)
    else:
        print("Odd Number", i)
    
```

    Even Number 12
    Odd Number 7
    Odd Number 25
    Odd Number 3
    Even Number 18
    Odd Number 9
    Even Number 30
    Even Number 14
    Even Number 6
    Odd Number 21



```python
    # print ("sq value", i ** 2)
sq_value = [i ** 2 for i in pythonnumbers]

print(sq_value)
```

    [144, 49, 625, 9, 324, 81, 900, 196, 36, 441]



```python
for i in pythonnumbers:
    if i%2 == 0:
        print("Even Number", i)
  
```

    Even Number 12
    Even Number 18
    Even Number 30
    Even Number 14
    Even Number 6



```python
pythonnumbers = [12, 7, 25, 3, 18, 9, 30, 14, 6, 21]
x = len(pythonnumbers)

```


```python
pythonnumbers = [12, 7, 25, 3, 18, 9, 30, 14, 6, 21]

pythonnumbers.sort()
print(pythonnumbers)

pythonnumbers.sort(reverse=True)
print(pythonnumbers)
```

    [3, 6, 7, 9, 12, 14, 18, 21, 25, 30]
    [30, 25, 21, 18, 14, 12, 9, 7, 6, 3]



```python
if 100 in pythonnumbers:
    print("100 is present")

else:
    print("100 is missing")
```

    100 is present



```python

```


---
**Score: 5**