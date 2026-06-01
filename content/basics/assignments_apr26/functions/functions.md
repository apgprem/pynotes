---
title: Functions
date: 2026-06-01
author: Your Name
cell_count: 5
score: 5
---

```python
def complete_profile(*args, **kwargs):
    print("Positional:", args)
    print("Keyword:", kwargs)

complete_profile("Python", level="Advanced", year=2025)
```

    Positional: ('Python',)
    Keyword: {'level': 'Advanced', 'year': 2025}



```python
def display_profile(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

display_profile(name="Alice", role="Engineer")
```

    name: Alice
    role: Engineer



```python
square = lambda x: x ** 3
print(square(5))  # Output: 25
```

    125



```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

    120



```python

```


---
**Score: 5**