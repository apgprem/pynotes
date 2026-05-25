---
title: Assign1
date: 2026-05-25
author: Your Name
cell_count: 9
score: 5
---

Assignment 1: Grocery List Manager (Basics)
Topics covered: Creating lists, indexing, append, remove, len
Task: Build a simple grocery list manager.

Create an empty list called grocery.
Add the following items one by one using append(): "milk", "bread", "eggs", "butter", "cheese".
Print the first item and the last item using indexing.
Remove "butter" from the list using remove().
Print the total number of items remaining using len().
Check if "bread" is in the list and print True or False.

Expected output sample:
First: milk
Last: cheese
Total items: 4
Bread in list: True


```python
grocery  = []
```


```python
print(grocery)
```

    []



```python
grocery.append("milk")
grocery.append("bread")
grocery.append("eggs")
grocery.append("butter")
grocery.append("cheese")


# grocery[1:4] = ("bread","eggs", "butter", "cheese")

print (grocery)

```

    ['milk', 'bread', 'eggs', 'butter', 'cheese']



```python
# grocery[1:4] = ("bread","eggs", "butter", "cheese")

print (grocery)
print (grocery[0])
print (grocery[-1])
# print (grocery_list)
```

    ['milk', 'bread', 'eggs', 'butter', 'cheese']
    milk
    cheese



```python

grocery.remove("butter")

print (grocery)

```

    ['milk', 'bread', 'eggs', 'cheese']



```python
print (grocery)
print (len(grocery))

```

    ['milk', 'bread', 'eggs', 'cheese']
    4



```python
if "bread" in grocery:
    print ("true")
else:
    print("false")
```

    true



```python

```


---
**Score: 5**