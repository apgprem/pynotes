---
title: Inheritance
date: 2026-06-01
author: Your Name
cell_count: 10
score: 10
---

```python
# 1. What is Inheritance - Inheritance allows a class (child) to acquire properties and behaviors of another class (parent).
# - Promotes code reusability and hierarchical design.

class Animal:
    def eat(self):
        print("Animal is eating")

class Dog(Animal):
    pass

d = Dog()
d.eat()  # Inherited method
```

    Animal is eating



```python
# 2. Single Inheritance - A child class inherits from one parent class.

class Parent:
    def show(self):
        print("This is the parent class")

class Child(Parent):
    pass

c = Child()
c.show()
```

    This is the parent class



```python
# 3. Adding New Methods in Child Class - Child classes can extend functionality beyond the parent.

class Animal:
    def sound(self):
        print("Some sound")

class Dog(Animal):
    def bark(self):
        print("Dog barks")

d = Dog()
d.sound()
d.bark()
```

    Some sound
    Dog barks



```python
# 4. Method Overriding - Child class can redefine parent methods.

class Animal:
    def sound(self):
        print("Animal makes sound")

class Dog(Animal):
    def sound(self):
        print("Dog barks")

d = Dog()
d.sound()  # Dog barks
```

    Dog barks



```python
# 5. Using super() to Call Parent Method - super() invokes the parent class method within the child.
class Animal:
    def sound(self):
        print("Animal makes sound")

class Dog(Animal):
    def sound(self):
        super().sound()
        print("Dog barks")

d = Dog()
d.sound()
```

    Animal makes sound
    Dog barks



```python
# 7. Multiple Inheritance - A child class inherits from multiple parent classes.

class Grandparent:
    def feature(self):
        print("Grandparent feature")

class Parent(Grandparent):
    pass

class Child(Parent):
    pass

c = Child()
c.feature()
```

    Grandparent feature



```python
# 8. Method Resolution Order (MRO)

class A:
    def show(self):
        print("A")

class B(A):
    def show(self):
        print("B")

class C(B):
    pass

c = C()
c.show()
print(C.mro())

# MRO defines the order in which methods are resolved in inheritance.
```

    B
    [<class '__main__.C'>, <class '__main__.B'>, <class '__main__.A'>, <class 'object'>]



```python
# 9. Constructor Inheritance - Child constructors can call parent constructors using super().

class Parent:
    def __init__(self, name):
        self.name = name

class Child(Parent):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

c = Child("Alice", 25)
print(c.name, c.age)
```

    Alice 25



```python
# 10. Real-World Inheritance Example - Demonstrates inheritance in an object-oriented system.

class Vehicle:
    def start(self):
        print("Vehicle started")

class Car(Vehicle):
    def drive(self):
        print("Car is driving")

class Bike(Vehicle):
    def ride(self):
        print("Bike is riding")

car = Car()
bike = Bike()

car.start()
car.drive()

bike.start()
bike.ride()
```

    Vehicle started
    Car is driving
    Vehicle started
    Bike is riding



```python

```


---
**Score: 10**