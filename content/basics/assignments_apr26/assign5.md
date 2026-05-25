---
title: Assign5
date: 2026-05-23
author: Your Name
cell_count: 10
score: 10
---

Assignment 5: Mini Library Catalog (Combined Operations)
Topics covered: Everything — creating, slicing, modifying, adding, removing, iterating, comprehension, sorting
Task: Build a small library catalog system.

Create a list of 6 book titles:

python   library = ["Python 101", "Data Structures", "Web Dev", "AI Basics", "ML Guide", "Networking"]

Print the catalog using a for loop with each book numbered (e.g., 1. Python 101).
A new book "Cloud Computing" arrives — add it at index 2.
The book "Networking" is no longer available — remove it.
Use a list comprehension to create a new list short_titles containing only books with fewer than 10 characters in their title.
Sort the library alphabetically and print it.
Slice and print only the middle 3 books of the sorted library.
Finally, print the total number of books in the catalog.

Bonus challenge: Use a list comprehension to create upper_titles where every book title is in UPPERCASE.


```python
library = ["Python 101", "Data Structures", "Web Dev", "AI Basics", "ML Guide", "Networking"]

for i in library:
    print (i)
```

    Python 101
    Data Structures
    Web Dev
    AI Basics
    ML Guide
    Networking



```python
library[2]="Cloud Computing"
print(library)
```

    ['Python 101', 'Data Structures', 'Cloud Computing', 'AI Basics', 'ML Guide', 'Networking']



```python
library.remove("Networking")
print(library)
```

    ['Python 101', 'Data Structures', 'Cloud Computing', 'AI Basics', 'ML Guide']



```python
library = ["Python 101", "Data Structures", "Web Dev", "AI Basics", "ML Guide", "Networking"]
# len_lib = len(library)
# print(len_lib)
short_titles = [book for book in library 
                    if len(book) < 10]

print(short_titles)
```

    ['Web Dev', 'AI Basics', 'ML Guide']



```python
library.sort()
print(library)
```

    ['AI Basics', 'Data Structures', 'ML Guide', 'Networking', 'Python 101', 'Web Dev']



```python
library.sort()
print(library[2:5])
```

    ['ML Guide', 'Networking', 'Python 101']



```python
# library.count()
print(len(library))
```

    6



```python
# print(upper(library))
library = ["Python 101", "Data Structures", "Web Dev", "AI Basics", "ML Guide", "Networking"]
upperlib = [books.upper() for books in library]
print(upperlib)
```

    ['PYTHON 101', 'DATA STRUCTURES', 'WEB DEV', 'AI BASICS', 'ML GUIDE', 'NETWORKING']



```python

```


---
**Score: 10**