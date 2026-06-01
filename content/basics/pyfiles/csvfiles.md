---
title: Csvfiles
date: 2026-06-01
author: Your Name
cell_count: 14
score: 10
---

```python
# 1. What is a CSV File

# A CSV (Comma-Separated Values) file stores tabular data in plain text, where each line represents a row and values are separated by commas.

# Example:


# name,age,city
# Alice,25,New York
# Bob,30,London
```


```python
# 2. Reading a CSV File Using csv.reader

import csv
with open("data1.csv", "w") as file:
    # file.write("""name,age,city
Alice,25,New York
Bob,30,London)
    file.update(
with open("data.csv", "r") as file:
    read_file = csv.reader(file)
    for row in read_file:
        print(row)

# Reads each row as a list of values.
```


      Cell In[5], line 7
        Bob,30,London""")
                     ^
    SyntaxError: unterminated triple-quoted string literal (detected at line 14)




```python
import csv

with open("user.csv", "w", newline='') as file:
    w = csv.writer(file)
    w.writerow(['name', 'age', 'city'])
    w.writerow(['Alice', 30, 'New York'])
    w.writerow(['Bob', 40, 'London'])

with open('user.csv', 'r') as f:
    rows = csv.reader(f)
    for row in rows:
        print(row)
```

    ['name', 'age', 'city']
    ['Alice', '30', 'New York']
    ['Bob', '40', 'London']



```python
import csv

data = [
    ["John", 28, "Toronto"],
    ["Emma", 35, "Berlin"]
]

with open("people.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerows(data)

with open("people.csv", "r") as file1:
    writer1 = csv.reader(file1)   
    for row in writer1:
        print(row)
```

    ['John', '28', 'Toronto']
    ['Emma', '35', 'Berlin']



```python
# 3. Skipping Header Row

import csv

with open("user.csv", "r") as file:
    reader = csv.reader(file)
    next(reader)  # Skip header
    for row in reader:
        print(row)
```

    ['Alice', '30', 'New York']
    ['Bob', '40', 'London']



```python
# 4. Reading CSV as Dictionary (csv.DictReader)

import csv

with open("user.csv", "r") as file:
    reader = csv.DictReader(file)
    for row in reader:
        print(row["name"], row["age"])
```

    Alice 30
    Bob 40



```python
# 5. Writing to a CSV File Using csv.writer

import csv

with open("output.csv", "a", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["Prem", 30, "London"])

with open("output.csv", "r") as file1:
    writer1 = csv.reader(file1)   
    for row in writer1:
        print(row)
```

    ['Prem', '30', 'London']
    ['Prem', '30', 'London']



```python
# 6. Writing Multiple Rows at Once

import csv

data = [
    ["John", 28, "Toronto"],
    ["Emma", 35, "Berlin"]
]

with open("people.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerows(data)

# Efficient for bulk data writing.
```


```python
# 7. Writing Dictionaries Using csv.DictWriter

import csv

fieldnames = ["name", "age", "city"]

with open("users.csv", "w", newline="") as file:
    writer = csv.DictWriter(file, fieldnames=fieldnames)
    writer.writeheader()
    
    writer.writerow({"name": "Alice", "age": 25, "city": "Paris"})
    writer.writerow({"name": "Bob", "age": 30, "city": "Rome"})
```


```python
# 8. Custom Delimiters and Quoting

import csv

with open("custom.csv", "w", newline="") as file:
    writer = csv.writer(file, delimiter="|")
    writer.writerow(["Name", "Age", "Country"])
    writer.writerow(["Alice", 25, "India"])

# CSV supports configurable delimiters for complex data formats.
```


```python
# 9. Appending Data to an Existing CSV

import csv

with open("users.csv", "a", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["Charlie", 40, "USA"])

# "a" mode appends data without overwriting existing rows.
```


```python
# 10. Reading CSV Using pandas (Advanced)

import pandas as pd

df = pd.read_csv("data.csv")
print(df.head())

# Pandas provides high-level, efficient CSV data manipulation for analytics and ML workflows.
```


    ---------------------------------------------------------------------------

    ModuleNotFoundError                       Traceback (most recent call last)

    Cell In[31], line 3
          1 # 10. Reading CSV Using pandas (Advanced)
          2 
    ----> 3 import pandas as pd
          4 
          5 df = pd.read_csv("data.csv")
          6 print(df.head())


    ModuleNotFoundError: No module named 'pandas'



```python
def safe_int_convert(value: str) -> int:
    try:
        return int(value)
    except ValueError:
        print(f"Cannot convert '{value}' to int. Defaulting to 0.")
        return 0

print(safe_int_convert("123"))   # Output: 123
print(safe_int_convert("2"))   # Output: Cannot convert 'abc' to int. Defaulting to 0.
                                 #         0
```

    123
    2



```python

```


---
**Score: 10**