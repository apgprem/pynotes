---
title: Untitled
date: 2026-05-23
author: Your Name
cell_count: 10
score: 10
---

```python
import os

current_dir = os.getcwd()
print(current_dir)
```

    /home/prem/kact/pynotes/notebooks/basics



```python
import os

os.chdir("C:/Projects")
print(os.getcwd())
```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    Cell In[1], line 3
          1 import os
          2 
    ----> 3 os.chdir("C:/Projects")
          4 print(os.getcwd())


    FileNotFoundError: [Errno 2] No such file or directory: 'C:/Projects'



```python
import os

print(os.path.exists("data.txt"))      # True or False
print(os.path.isfile("data.txt"))     # Checks file
print(os.path.isdir("new_folder"))    # Checks directory
```

    False
    False
    True



```python
import os

os.mkdir("new_folder")
```


```python
with open("source.txt", "w") as file:
    file.write("Hello, Python File System")
```


```python
with open("sample.txt", "r") as file:
    content = file.read()

print(content)
```

    Hello, Python File System



```python
import os

# os.rename("sample.txt", "renamed.txt")
os.remove("renamed.txt")
```


```python
import shutil

shutil.copy("source.txt", "backup.txt")
shutil.move("backup.txt", "backup1.txt")
```




    'backup1.txt'




```python
from pathlib import Path

file_path = Path("example.txt")

file_path.write_text("Using pathlib module")
print(file_path.read_text())

print(file_path.exists())
print(file_path.parent)
```

    Using pathlib module
    True
    .



```python

```


---
**Score: 10**