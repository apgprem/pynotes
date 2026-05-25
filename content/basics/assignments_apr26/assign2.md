---
title: Assign2
date: 2026-05-25
author: Your Name
cell_count: 9
score: 5
---

Assignment 2: Student Marks Slicer (Indexing & Slicing)
Topics covered: Slicing, negative indexing, modifying elements
Task: A teacher has marks of 10 students stored in order.
pythonmarks = [78, 82, 65, 90, 45, 88, 73, 99, 60, 55]

Print the marks of the first 3 students using slicing.
Print the marks of the last 3 students using slicing.
Print the marks of students from index 3 to index 7 (inclusive of 3, exclusive of 8).
The 5th student (index 4) was re-evaluated and now has 70 instead of 45 — update it.
Print every alternate student's marks using slicing with a step (e.g., marks[::2]).


```python
pythonmarks = [78, 82, 65, 90, 45, 88, 73, 99, 60, 55]
print (pythonmarks[:3])
```

    [78, 82, 65]



```python
print (pythonmarks[-3:])
```

    [99, 60, 55]



```python
print (pythonmarks[3:8])
```

    [90, 45, 88, 73, 99]



```python
pythonmarks[4] = 70
print (pythonmarks)
```

    [78, 82, 65, 90, 70, 88, 73, 99, 60, 55]



```python
print ("alternative students marks")
print (pythonmarks[::2])
```

    alternative students marks
    [78, 65, 70, 73, 60]



```python
print ("alternative students marks", pythonmarks[::2])

```

    alternative students marks [78, 65, 70, 73, 60]



```python

```


```python

```


---
**Score: 5**