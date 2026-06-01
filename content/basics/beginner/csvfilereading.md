---
title: Csvfilereading
date: 2026-06-01
author: Your Name
cell_count: 9
score: 5
---

```python
import csv

with open("abc.csv", "r") as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)
```

    ['name', 'age', 'city']
    ['Alice', '25', 'New York']
    ['Bob', '30', 'London']



```python
import csv

with open("abc.csv", "r") as file:
    reader = csv.reader(file)
    next(reader)  # Skip header
    for row in reader:
        print(row)
```

    ['Alice', '25', 'New York']
    ['Bob', '30', 'London']



```python
import csv

with open("output.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["name", "age", "city"])
    writer.writerow(["Alice", 25, "New York"])
    writer.writerow(["Bob", 30, "London"])
```


```python
import csv

data = [
    ["John", 28, "Toronto"],
    ["Emma", 35, "Berlin"]
]

with open("people.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerows(data)
```


```python
import csv

fieldnames = ["name", "age", "city"]

with open("users.csv", "w", newline="") as file:
    writer = csv.DictWriter(file, fieldnames=fieldnames)
    writer.writeheader()
    
    writer.writerow({"name": "Alice", "age": 25, "city": "Paris"})
    writer.writerow({"name": "Bob", "age": 30, "city": "Rome"})
```


```python
import csv

with open("custom.csv", "w", newline="") as file:
    writer = csv.writer(file, delimiter="|")
    writer.writerow(["Name", "Age", "Country"])
    writer.writerow(["Alice", 25, "India"])
```


```python
import csv

with open("users.csv", "a", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["Charlie11", 40, "USA"])
```


```python
import pandas as pd

df = pd.read_csv("data.csv")
print(df.head())
```


    ---------------------------------------------------------------------------

    ModuleNotFoundError                       Traceback (most recent call last)

    Cell In[17], line 1
    ----> 1 import pandas as pd
          2 
          3 df = pd.read_csv("data.csv")
          4 print(df.head())


    ModuleNotFoundError: No module named 'pandas'



```python

```


---
**Score: 5**