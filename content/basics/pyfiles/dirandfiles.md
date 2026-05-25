---
title: Dirandfiles
date: 2026-05-23
author: Your Name
cell_count: 10
score: 10
---

```python
# 1. Getting Current Working Directory

import os

current_dir = os.getcwd()
print(current_dir)
```

    /home/prem/kact/pynotes/notebooks/basics



```python
# 2. Changing the Working Directory

# import os

# os.chdir("C:/Projects")
# print(os.getcwd())
```


```python
# 3. Listing Files and Directories

import os

items = os.listdir(".")
print(items)
```

    ['variable_assignment.ipynb', 'recursion.ipynb', 'assignments_apr26', '.ipynb_checkpoints', 'ioop.ipynb', 'globalkeyword.ipynb', 'forloop.ipynb', 'ifs.ipynb', 'variable_conv_assignment.ipynb', 'functions', 'operators.ipynb', 'pythonfiles', 'output.txt', 'pythonexcephandling', 'hello.ipynb', 'age-calculator.ipynb']



```python
# 4. Creating a Directory

import os

# os.mkdir("India")
# os.makedirs("parent/child/grandchild")

items = os.listdir(".")
print(items)
```

    ['variable_assignment.ipynb', 'recursion.ipynb', 'assignments_apr26', '.ipynb_checkpoints', 'ioop.ipynb', 'globalkeyword.ipynb', 'forloop.ipynb', 'India', 'ifs.ipynb', 'variable_conv_assignment.ipynb', 'functions', 'parent', 'operators.ipynb', 'pythonfiles', 'output.txt', 'pythonexcephandling', 'hello.ipynb', 'age-calculator.ipynb']



```python
# 5. Checking File or Directory Existence

import os

print(os.path.exists("data.txt"))      # True or False
print(os.path.isfile("data.txt"))     # Checks file
print(os.path.isdir("India"))    # Checks directory
```

    False
    False
    True



```python
# 6. Creating and Writing to a File

with open("sample.txt", "w") as file:
    file.write("Hello, Python File System")
```


```python
# 7. Reading from a File

with open("sample1.txt", "r") as file:
    content = file.read()

print(content)
```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    Cell In[1], line 3
          1 # 7. Reading from a File
          2 
    ----> 3 with open("sample1.txt", "r") as file:
          4     content = file.read()
          5 
          6 print(content)


    FileNotFoundError: [Errno 2] No such file or directory: 'sample1.txt'



```python
# 8. Renaming and Deleting Files

import os

os.rename("renamed.txt","sample.txt")
# os.remove("renamed.txt")
```


```python
# 9. Copying and Moving Files

import shutil

shutil.copy("source.txt", "backup.txt")
shutil.move("backup.txt", "archive/backup.txt")

# Provides advanced file handling capabilities.

```


```python
# 10. Modern File Handling with pathlib

from pathlib import Path

file_path = Path("example.txt")

file_path.write_text("Using pathlib module")
print(file_path.read_text())

print(file_path.exists())
print(file_path.parent)

# pathlib offers an object-oriented and cleaner approach for file and directory manipulation.
```


---
**Score: 10**