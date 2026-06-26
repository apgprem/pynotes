---
title: Multipleinherit-3423
date: 2026-06-26
author: Your Name
cell_count: 11
score: 10
---

```python
# 1. What is Multiple Inheritance - Multiple inheritance occurs when a class inherits from more than one parent class.
class Father:
    def skill1(self):
        print("Driving")

class Mother:
    def skill2(self):
        print("Cooking")

class Child(Father, Mother):
    pass

c = Child()
c.skill1()
c.skill2()

# - The child class gains features from all parent classes.
```

    Driving
    Cooking



```python
# 2. Basic Multiple Inheritance Structure
# The child class can access methods from both parents.
class A:
    def show_a(self):
        print("Class A")

class B:
    def show_b(self):
        print("Class B")

class C(A, B):
    pass

obj = C()
obj.show_a()
obj.show_b()
```

    Class A
    Class B



```python
# 3. Overlapping Method Names
# Python follows Method Resolution Order (MRO) to determine which method to invoke.
class A:
    def display(self):
        print("From A")

class B:
    def display(self):
        print("From B")

class C(A, B):
    pass

obj = C()
obj.display()
```

    From A



```python
# 4. Understanding Method Resolution Order (MRO)
class A:
    def show(self):
        print("A")

class B:
    def show(self):
        print("B")

class C(A, B):
    pass

print(C.mro())

# MRO defines the order of class traversal:
# C → A → B → object
```

    [<class '__main__.C'>, <class '__main__.A'>, <class '__main__.B'>, <class 'object'>]



```python
# 5. Calling Parent Methods Explicitly - Allows execution of logic from multiple parents.
class A:
    def process(self):
        print("Process A")

class B:
    def process(self):
        print("Process B")

class C(A, B):
    def process(self):
        A.process(self)
        B.process(self)

c = C()
c.process()
```

    Process A
    Process B



```python
# 6. Multiple Inheritance with Constructors
class A:
    def __init__(self):
        print("Constructor A")

class B:
    def __init__(self):
        print("Constructor B")

class C(A, B):
    def __init__(self):
        super().__init__()

c = C()

# Only the first parent’s constructor executes due to MRO.
```

    Constructor A



```python
# 7. Cooperative Multiple Inheritance Using super()
class A:
    def __init__(self):
        print("A init")
        super().__init__()

class B:
    def __init__(self):
        print("B init")
        super().__init__()

class C(A, B):
    def __init__(self):
        print("C init")
        super().__init__()

c = C()
# Demonstrates cooperative method chaining through MRO.
```

    C init
    A init
    B init



```python
# 8. Diamond Problem Example - Python resolves this ambiguity using MRO, avoiding duplicate calls.
class Grandparent:
    def greet(self):
        print("Hello from Grandparent")

class Parent1(Grandparent):
    pass

class Parent2(Grandparent):
    pass

class Child(Parent1, Parent2):
    pass

c = Child()
c.greet()
```

    Hello from Grandparent



```python
# 9. Visualizing the Inheritance Hierarchy - Helps understand order of class resolution for debugging.

class X:
    pass

class Y(X):
    pass

class Z(X):
    pass

class W(Y, Z):
    pass

print(W.mro())
```

    [<class '__main__.W'>, <class '__main__.Y'>, <class '__main__.Z'>, <class '__main__.X'>, <class 'object'>]



```python
# 10. Real-World Multiple Inheritance Example

class Logger:
    def log(self):
        print("Logging data")

class Validator:
    def validate(self):
        print("Validating data")

class Service(Logger, Validator):
    def execute(self):
        self.log()
        self.validate()
        print("Executing service")

service = Service()
service.execute()

# Combines cross-cutting concerns such as logging and validation.
```

    Logging data
    Validating data
    Executing service



```python

```


---
**Score: 10**