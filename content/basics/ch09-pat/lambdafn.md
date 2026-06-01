---
title: Lambdafn
date: 2026-06-01
author: Your Name
cell_count: 9
score: 5
---

```python
square = lambda x: x ** 2
print(square(5))  # Output: 25
```

    25



```python
add = lambda a, b: a + b
print(add(10, 5))  # Output: 15
```

    15



```python
print((lambda x, y: x * y)(4, 5))  # Output: 20
```

    20



```python
numbers = [1, 2, 3, 4]

squares = list(map(lambda x: x ** 2, numbers))
print(squares)  # Output: [1, 4, 9, 16]
```

    [1, 4, 9, 16]



```python
numbers = [1, 2, 3, 4, 5, 6]

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print(even_numbers)  # Output: [2, 4, 6]
```

    [2, 4, 6]



```python
from functools import reduce

numbers = [1, 2, 3, 4]

total = reduce(lambda x, y: x + y, numbers)
print(total)  # Output: 10
```

    10



```python
def square_func(x):
    return x ** 2

square_lambda = lambda x: x ** 2

print(square_func(4))     # 16
print(square_lambda(4))   # 16
```

    16
    16



```python
employees = [
    {"name": "Alice", "salary": 5000},
    {"name": "Bob", "salary": 3000},
    {"name": "Charlie", "salary": 7000}
]

highest_paid = max(employees, key=lambda emp: emp["salary"])
print(highest_paid)
```

    {'name': 'Charlie', 'salary': 7000}



```python

```


---
**Score: 5**