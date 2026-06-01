---
title: Assign7
date: 2026-06-01
author: Your Name
cell_count: 8
score: 5
---

Assignment 7: Password Validator List
Topics covered: Membership, iteration, list comprehension, conditions
Task: A system has a list of weak passwords that should be rejected.
pythonweak_passwords = ["123456", "password", "qwerty", "admin", "letmein", "welcome"]
user_attempts = ["hello123", "password", "MyP@ss99", "qwerty", "Strong#2026", "admin"]

Loop through user_attempts and for each attempt, print whether it is "REJECTED" (in weak list) or "ACCEPTED".
Use a list comprehension to create rejected — all attempts that exist in weak_passwords.
Use a list comprehension to create accepted — all attempts that are not in weak_passwords.
Print the count of rejected and accepted attempts.
Add "123456789" to weak_passwords using append(), then re-check "123456789" membership.


```python
pythonweak_passwords = ["123456", "password", "qwerty", "admin", "letmein", "welcome"]
user_attempts = ["hello123", "password", "MyP@ss99", "qwerty", "Strong#2026", "admin"]

for i in user_attempts:
    if i in pythonweak_passwords:
        print("REJECTED")

    else:
        print("Accepted")
```

    Accepted
    REJECTED
    Accepted
    REJECTED
    Accepted
    REJECTED



```python
for i in user_attempts:
    if i in pythonweak_passwords:
        print("REJECTED")
```

    REJECTED
    REJECTED
    REJECTED



```python
rejected_pwds = [attempts for attempts in user_attempts if attempts in pythonweak_passwords]
print(rejected_pwds)
```

    ['password', 'qwerty', 'admin']



```python
accepted_pwds = [attempts for attempts in user_attempts if attempts not in pythonweak_passwords]
print(accepted_pwds)
```

    ['hello123', 'MyP@ss99', 'Strong#2026']



```python
print(len(rejected_pwds))
print(len(accepted_pwds))
```

    3
    3



```python
pythonweak_passwords.append("123456789")
print(pythonweak_passwords)
```

    ['123456', 'password', 'qwerty', 'admin', 'letmein', 'welcome', '123456789']



```python

```


---
**Score: 5**