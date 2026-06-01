---
title: Variables
date: 2026-06-01
author: Your Name
cell_count: 13
score: 10
---

```python
name = "ada lovelace"
print(name.title())
```

    Ada Lovelace



```python
name = "Ada Lovelace"
print(name.upper())
print(name.lower())
```

    ADA LOVELACE
    ada lovelace



```python
first_name = "ada"
last_name = "lovelace"
full_name = first_name + " " + last_name
print(full_name)
```

    ada lovelace



```python
first_name = "ada"
last_name = "lovelace"
full_name = first_name + " " + last_name
print("Hello, " + full_name.title() + "!")
```

    Hello, Ada Lovelace!



```python
first_name = "ada"
last_name = "lovelace"
full_name = first_name + " " + last_name
message = "Hello, " + full_name.title() + "!"
print(message)
```

    Hello, Ada Lovelace!



```python
>>> print("Python")

>>> print("\tPython")

```

    Python
    	Python



```python
print("Languages:\nPython\nC\nJavaScript")
```

    Languages:
    Python
    C
    JavaScript



```python
>>> print("Languages:\n\tPython\n\tC\n\tJavaScript")
```

    Languages:
    	Python
    	C
    	JavaScript



```python
>>> favorite_language = 'python '
>>> favorite_language = favorite_language.rstrip()
>>> favorite_language
```




    'python'




```python
message = 'One of Python's strengths is its diverse community.'
print(message)
```


      Cell In[16], line 1
        message = 'One of Python's strengths is its diverse community.''
                                 ^
    SyntaxError: invalid syntax




```python
>>> 3 / 2
1
```




    1




```python
Say hello to everyone.
print("Hello Python people!")
```


      Cell In[19], line 1
        Say hello to everyone.
            ^
    SyntaxError: invalid syntax




```python

```


---
**Score: 10**