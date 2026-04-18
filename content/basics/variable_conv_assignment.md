---
title: Variable Conv Assignment
date: 2026-04-18
author: Your Name
cell_count: 16
score: 15
---

```python
# 1. Implicit Type Conversion (Type Coercion)

integer_value = 10       # int
float_value = 3.5       # float

result = integer_value + float_value  # int + float → float

print(result)           # Output: 13.5
print(type(result))     # Output: <class 'float'>
```

    13.5
    <class 'float'>



```python
float_value = 9.99
string_value = "42"

int_from_float = int(float_value)
int_from_string = int(string_value)

print(int_from_float)    # Output: 9   (fraction truncated)
print(int_from_string)   # Output: 42
```

    9
    42



```python
int_value = 7
string_value = "3.14"

float_from_int = float(int_value)
float_from_string = float(string_value)

print(float_from_int)      # Output: 7.0
print(float_from_string)   # Output: 3.14
```

    7.0
    3.14



```python
int_value = 100
float_value = 25.5
bool_value = True

str_int = str(int_value)
str_float = str(float_value)
str_bool = str(bool_value)

print(str_int)    # Output: '100'
print(str_float)  # Output: '25.5'
print(str_bool)   # Output: 'True'
```

    100
    25.5
    True



```python
print(bool(0))        # Output: False
print(bool(1))        # Output: True
print(bool(""))       # Output: False
print(bool("text"))   # Output: True
print(bool([]))       # Output: False
print(bool([1, 2]))   # Output: True
```

    False
    True
    False
    True
    False
    True



```python
text = "python"

# String to list of characters
char_list = list(text)
print(char_list)  # Output: ['p', 'y', 't', 'h', 'o', 'n']

# List of strings to single string
words = ["Python", "Type", "Conversion"]
joined = " ".join(words)
print(joined)     # Output: Python Type Conversion
```

    ['p', 'y', 't', 'h', 'o', 'n']
    Python Type Conversion



```python
numbers_list = [1, 2, 2, 3]

numbers_tuple = tuple(numbers_list)
numbers_set = set(numbers_list)

print(numbers_tuple)  # Output: (1, 2, 2, 3)
print(numbers_set)    # Output: {1, 2, 3}
```

    (1, 2, 2, 3)
    {1, 2, 3}



```python
pairs_list = [("a", 1), ("b", 2)]
pairs_tuple = (("x", 10), ("y", 20))

dict_from_list = dict(pairs_list)
dict_from_tuple = dict(pairs_tuple)

print(dict_from_list)   # Output: {'a': 1, 'b': 2}
print(dict_from_tuple)  # Output: {'x': 10, 'y': 20}
```

    {'a': 1, 'b': 2}
    {'x': 10, 'y': 20}



```python
def safe_int_convert(value: str) -> int:
    try:
        return int(value)
    except ValueError:
        print(f"Cannot convert '{value}' to int. Defaulting to 0.")
        return 0

print(safe_int_convert("123"))   # Output: 123
print(safe_int_convert("abc"))   # Output: Cannot convert 'abc' to int. Defaulting to 0.
                                 #         0
```

    123
    Cannot convert 'abc' to int. Defaulting to 0.
    0



```python
class Score:
    def __init__(self, points: int):
        self.points = points

    def __str__(self) -> str:
        return f"Score: {self.points}"

    def __int__(self) -> int:
        return self.points

player_score = Score(95)

print(str(player_score))  # Output: Score: 95
print(int(player_score))  # Output: 95
```

    Score: 95
    95



```python
list = ("Raj", "Krish", "Shiv")
print(len(list))
```

    3



```python
list = ("Raj", "Krish", "Shiv")
    y = return (len(list))
print(y)
```


      Cell In[5], line 2
        y = return (len(list))
        ^
    IndentationError: unexpected indent




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
def list(a, b, c)
    
```


```python

```


---
**Score: 15**