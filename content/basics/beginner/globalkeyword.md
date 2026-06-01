---
title: Globalkeyword
date: 2026-06-01
author: Your Name
cell_count: 16
score: 15
---

```python
value = 5

def update():
    value = value + 1  # UnboundLocalError
```


```python
counter = 0

def increment():
    global counter
    counter += 1

increment()
print(counter)  # Output: 1
```


```python
status = "inactive"

def activate():
    global status
    status = "active"

def show_status():
    print(status)

activate()
show_status()  # Output: active
```

    active



```python
# 1 Basic Use of Global Variable

count = 10

def display():
    # count = 101
    print(count)

display()  # Output: 10
```

    101



```python
# 2. Modifying Global Variable Without global (Error Case)

counter = 1

def increment():
    global counter
    counter += 3

increment()
print(counter)  # Output: 1
```

    4



```python
# 4. Global Variable Across Multiple Functions

status = "inactive"

def activate():
    global status
    status = "active"

def show_status():
    print(status)

activate()
show_status()  # Output: active

```

    active



```python
# 5. Global Keyword Inside Nested Functions

x = 100

def outer():
    def inner():
        global x
        x = 200

    inner()

outer()
print(x)  # Output: 200
```

    200



```python
# 6. Difference Between global and nonlocal

x = 50

def outer():
    x = 10
    
    def inner():
        global x
        x = 99

    inner()
    print("Outer x:", x)

outer()
print("Global x:", x)
```

    Outer x: 10
    Global x: 99



```python
# 7. Tracking State Using Global Variable

requests = 0

def handle_request():
    global requests
    requests += 1

handle_request()
handle_request()
handle_request()
print(requests)  # Output: 2
```

    3



```python
# 8. Global Variable with Conditional Logic

mode = "dark"

def toggle_mode():
    global mode
    if mode == "light":
        mode = "dark"
    else:
        mode = "light"

toggle_mode()
print(mode)  # Output: dark
```

    light



```python
# 9. Avoiding Global Abuse (Best Practice Warning)

config = {"theme": "dark"}

def update_config(new_theme):
    config["theme"] = new_theme  # No global keyword needed
```


```python
# 10. Best Practice: Encapsulation Instead of Global

class Counter:
    def __init__(self):
        self.value = 1.5

    def increment(self):
        self.value += 1

counter = Counter()
counter.increment()
print(counter.value)  # Output: 1
```

    2.5



```python

```


```python

```


```python

```


```python

```


---
**Score: 15**