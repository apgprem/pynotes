---
title: Listcomprehension
date: 2026-06-26
author: Your Name
cell_count: 18
score: 15
---

```python
squares = [x**2 for x in range(5)]
print(squares)
```

    [0, 1, 4, 9, 16]



```python
squares = []
for x in range(5):
    squares.append(x**2)

print(squares)
```

    [0, 1, 4, 9, 16]



```python
even_numbers = [x for x in range(10) if x % 2 == 0]

print(even_numbers)
```

    [0, 2, 4, 6, 8]



```python
def transform(x):
    return x * 10

result = [transform(x) for x in range(5)]

print(result)
```

    [0, 10, 20, 30, 40]



```python
matrix = [[i * j for j in range(3)] for i in range(3)]

print(matrix)
```

    [[0, 0, 0], [0, 1, 2], [0, 2, 4]]



```python
result = [x for x in range(20) if x > 5 if x % 2 == 0]

print(result)
```

    [6, 8, 10, 12, 14, 16, 18]



```python
status = ["even" if x % 2 == 0 else "odd" for x in range(5)]

print(status)
```

    ['even', 'odd', 'even', 'odd', 'even']



```python
(x**2 for x in range(10))
```




    <generator object <genexpr> at 0x78ba5015b2a0>




```python
nested = [[1, 2], [3, 4], [5]]
flat = [item for sublist in nested for item in sublist]

print(flat)
```

    [1, 2, 3, 4, 5]



```python
raw = ["  apple ", " Banana", "cherry "]
cleaned = [item.strip().lower() for item in raw]

print(cleaned)
```

    ['apple', 'banana', 'cherry']



```python
pairs = [(x, y) for x, y in zip([1,2], [3,4])]

print(pairs)
```

    [(1, 3), (2, 4)]



```python
keys = ["a", "b"]
values = [1, 2]
data = {k: v for k, v in zip(keys, values)}

print(data)
```

    {'a': 1, 'b': 2}



```python
keys = ["a", "b"]
values = [1, 2]
data = {k: v for k, v in zip(keys, values)}

print(data)
```

    {'a': 1, 'b': 2}



```python
active_users = [u for u in users if u.is_active]

print(active_users)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[20], line 1
    ----> 1 active_users = [u for u in users if u.is_active]
          2 
          3 print(active_users)


    NameError: name 'users' is not defined



```python
indexed = [(i, v) for i, v in enumerate(["a", "b", "c"])]

print(indexed)
```

    [(0, 'a'), (1, 'b'), (2, 'c')]



```python
unique = {x for x in [1,2,2,3]}
mapped = {x: x**2 for x in range(5)}

print(unique)
print(mapped)
```

    {1, 2, 3}
    {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}



```python
pipeline = [x * 2 for x in data if x > 0]

print(pipeline)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[24], line 1
    ----> 1 pipeline = [x * 2 for x in data if x > 0]
          2 
          3 print(pipeline)


    TypeError: '>' not supported between instances of 'str' and 'int'



```python

```


---
**Score: 15**