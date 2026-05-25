---
title: Objnclasses
date: 2026-05-25
author: Your Name
cell_count: 11
score: 10
---

```python
# 1. What is a Class and an Object
#        A class is a blueprint for creating objects. An object is an instance of a class.
# Classes define structure; objects represent real entities.

class Person:
    pass

p1 = Person()
print(p1)
```

    <__main__.Person object at 0x7d6d9023e2d0>



```python
# 2. Defining a Class with Attributes - Attributes represent properties of the class.
class Person:
    name = "Alice"
    age = 25

p = Person()
print(p.name)
print(p.age)
```

    Alice
    25



```python
# 3. Constructor Method (__init__) - The constructor initializes object data at creation.
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p = Person("Bob", 30)
print(p.name, p.age)
```

    Bob 30



```python
# 4. Instance Methods - Instance methods operate on object data using self.

class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        return f"Hello, my name is {self.name}"

p = Person("Alice")
print(p.greet())
```

    Hello, my name is Alice



```python
# 5. Class Variables vs Instance Variables
       # - Class variables are shared
       # - Instance variables are unique per object

class Student:
    school = "Global Academy"  # Class variable

    def __init__(self, name):
        self.name = name        # Instance variable

s1 = Student("Alice")
s2 = Student("Bob")

print(s1.name, s1.school)
print(s2.name, s2.school)
```

    Alice Global Academy
    Bob Global Academy



```python
# 6. Creating Multiple Objects
# Multiple objects can be created from the same class.

class Car:
    def __init__(self, brand):
        self.brand = brand

c1 = Car("Toyota")
c2 = Car("Tesla")

print(c1.brand)
print(c2.brand)
```

    Toyota
    Tesla



```python
# 7. Modifying Object Properties
#  Objects allow runtime modification of attributes.
class Employee:
    def __init__(self, name):
        self.name = name

emp = Employee("John")
emp.name = "Michael"

print(emp.name)
```

    Michael



```python
# 8. Deleting Object Properties and Objects - Use del to remove attributes or the object itself.
# del item  # Deletes the object entirely
class Product:
    def __init__(self, price):
        self.price = price

item = Product(100)

# del item.price

```


```python
# 9. Built-in Object Functions

class User:
    pass

user = User()

print(isinstance(user, User))  # True
print(type(user))              # <class '__main__.User'>


# Common object-related built-ins:

# type()
# isinstance()
```

    True
    <class '__main__.User'>



```python
# 10. Real-World Class Example - Encapsulation of data and behavior into a single unit.

class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount

    def withdraw(self, amount):
        self.balance -= amount

account = BankAccount("Alice", 1000)
account.deposit(500)
print(account.balance)  # Output: 1500
```

    1500



```python

```


---
**Score: 10**