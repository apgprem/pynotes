---
title: Assign3
date: 2026-06-26
author: Your Name
cell_count: 9
score: 5
---

ssignment 3: To-Do List with Insert and Pop (Add/Remove Operations)
Topics covered: append(), insert(), pop(), remove()
Task: Simulate a to-do list workflow.

Start with: todo = ["write report", "send email", "call client"]
Add "review code" at the end using append().
Add "morning standup" at the very beginning (index 0) using insert().
The user finished the first task — remove the item at index 0 using pop() and store it in a variable called completed.
Cancel the task "send email" using remove().
Print the final to-do list and print f"Completed task: {completed}".

Bonus: Print the list in reverse order without modifying it (hint: slicing with [::-1]).


```python
todo = ["write report", "send email", "call client"]
```


```python
todo = ["write report", "send email", "call client"]
todo.append("review code")
print(todo)
```

    ['write report', 'send email', 'call client', 'review code']



```python
todo.insert(0, "morning standup")
print(todo)
```

    ['morning standup', 'write report', 'send email', 'call client', 'review code']



```python
completed = todo.pop(0)
print(completed)
```

    morning standup



```python
todo.remove("send email")
print(todo)
```

    ['write report', 'call client', 'review code']



```python
print("Final to-do list", todo)
print(f"completed task: {completed}")
```

    Final to-do list ['write report', 'call client', 'review code']
    completed task: morning standup



```python
print(todo[::-1])
```

    ['review code', 'call client', 'write report']



```python

```


---
**Score: 5**