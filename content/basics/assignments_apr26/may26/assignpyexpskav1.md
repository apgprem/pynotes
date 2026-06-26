---
title: Assignpyexpskav1
date: 2026-06-26
author: Your Name
cell_count: 21
score: 20
---

Assignment 1 — Basic Safety Net
Write a program that asks the user to enter two numbers and divides them. Handle ZeroDivisionError and ValueError (for non-numeric input) separately, printing a clear message for each case.


```python
try:
    value = int("10")
    result = value / 0
except ValueError:
    print("Conversion error")
except ZeroDivisionError:
    print("Division error")
```

    Division error


Assignment 2 — File Reader with Cleanup
Write a function read_file(filename) that opens and reads a file. Use finally to always print "File operation complete", and handle FileNotFoundError with a friendly message. Test it with both a valid and an invalid filename.


```python
try:
    file = open("data1.txt", "r")
except FileNotFoundError:
    print("File not found")
finally:
    print("File Operation complete")
```

    File not found
    File Operation complete


Assignment 3 — The else Clause
Write a function parse_and_double(value) that converts a string to an integer. Use the else block to double the number and print it only if conversion succeeds. Handle ValueError in the except block.


```python
try:
    value = 45
    strvalue = str(value)
except ValueError:    
    print("value error")
    
else:
    mulvalue = value * 2
    print(mulvalue)
    
```

    90


Assignment 4 — Multi-Exception Handler
Write a function smart_access(data, index) that accepts a list and an index, then returns data[index] converted to an integer. Handle IndexError, ValueError, and TypeError each with a unique message.


```python

```

Assignment 5 — Custom Exception
Create a custom exception InsufficientFundsError. Write a BankAccount class with a withdraw(amount) method that raises this exception if the withdrawal exceeds the balance. Catch and display the error in a try...except block.


```python
try: 
    withdrawamt = 25
    withdrawamt >=20:
except InsufficientFundsError:
        print("In Suf bal")
```


      Cell In[34], line 3
        withdrawamt >=20:
                        ^
    SyntaxError: invalid syntax




```python
age = 15
assert age >= 18, "User must be at least 18 years old"
```


    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    Cell In[31], line 2
          1 age = 15
    ----> 2 assert age >= 18, "User must be at least 18 years old"


    AssertionError: User must be at least 18 years old


Assignment 6 — Re-raise with Logging
Write a function load_config(filepath) that opens a JSON config file. If a FileNotFoundError occurs, print "Logging: config file missing" and then re-raise the exception. Call it inside another try...except that catches the re-raised error and prints "App cannot start without config."


```python
try:
    file = open("data1.json", "r")
except FileNotFoundError:
    print("Logging: config file missing")
    
finally:
    print("File Operation complete")
```

    Logging: config file missing
    File Operation complete


Assignment 7 — Nested Exception Handling
Write a program that reads a list of strings and, for each item, tries to convert it to a float and then takes its square root (manually, without math). Use nested try...except blocks — the inner one handles ValueError, the outer one handles negative number cases with a custom exception.



```python

```

Assignment 8 — Assertion-Based Validator
Write a function register_user(username, age, email) that uses assert statements to validate: username is non-empty, age is between 18 and 100, and email contains @. Test it by calling the function with invalid inputs and observe the AssertionError messages.


```python

```

Assignment 9 — Production-Grade Calculator
Build a calculator(a, op, b) function that supports +, -, *, /. Handle ZeroDivisionError, TypeError, and an invalid operator using a custom InvalidOperatorError. Use a finally block to log every operation attempt regardless of outcome.


```python

```

Assignment 10 — Exception Chain & Hierarchy
Create a mini exception hierarchy: a base class AppError, and two subclasses DatabaseError and NetworkError. Write a function fetch_data(source) that raises DatabaseError if source is "db" and NetworkError if source is "api". In the calling code, catch AppError (the parent) and print which specific subclass was raised using type(e).__name__. Test with both sources.


```python

```


---
**Score: 20**