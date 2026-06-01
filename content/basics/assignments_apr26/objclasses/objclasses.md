---
title: Objclasses
date: 2026-06-01
author: Your Name
cell_count: 13
score: 10
---

```python
class dog:
    name = "tiger"
    breed = "Kombai"

d = dog()
# print(str(d))
print(d.name)
print(d.breed)
```

    tiger
    Kombai



```python
class book:
    def __init__(self, title, author):
        self.title = title
        self.author = author

    def display(self):
        # print(f"Title is:{self.title}")
        # print(f"Author is: {self.author}")

        print(f"Title and Author is:{self.title}, {self.author}")


b1 = book("My Python", "Prem")
b2 = book("FastAPI","FastAPI by prem")

print("Book1 details")
b1.display()

print("Book2 details")
b2.display()


```

    Book1 details
    Title and Author is:My Python, Prem
    Book2 details
    Title and Author is:FastAPI, FastAPI by prem



```python
class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = author


book1 = Book("The God of Small Things", "Arundhati Roy")
book2 = Book("Midnight's Children", "Salman Rushdie")

print(f"Book 1: {book1.title} by {book1.author}")
print(f"Book 2: {book2.title} by {book2.author}")
```

    Book 1: The God of Small Things by Arundhati Roy
    Book 2: Midnight's Children by Salman Rushdie



```python
class circle:
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius

c = circle(5)

print(c.radius)
print(c.area())
```

    5
    78.5



```python
class Student:
    # def __init__(self, school)
    school = "Sunrise School"
    def __init__(self, student_name):
        self.student_name = student_name

s1 = Student("Aswin")
s2 = Student("Briha")
s3 = Student("Sarvatha")

print(f"{s1.school}, {s1.student_name}")
print(f"{s2.school}, {s2.student_name}")
print(f"{s3.school}, {s3.student_name}")
```

    Sunrise School, Aswin
    Sunrise School, Briha
    Sunrise School, Sarvatha



```python
class Laptop:
    def __init__(self, brand, price):
        self.brand = brand
        self.price = price

L1 = Laptop("HP", 60000)
L2 = Laptop("Dell", 70000)
L3 = Laptop("Mac", 150000)

print(f"{L1.brand}, {L1.price}")
print(f"{L2.brand}, {L2.price}")
print(f"{L3.brand}, {L3.price}")
```

    HP, 60000
    Dell, 70000
    Mac, 150000



```python
class Employee:
     def __init__(self, name, salary):
         self.name = name
         self.salary = salary

emp = Employee("Aswin", 25000)

emp.salary = 50000

print(f"{emp.name}, {emp.salary}")

```

    Aswin, 50000



```python
class person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def introduce(self):
        print(f"Hi, I am {self.name} and I am {self.age} years old.")
        # print(f"Hi, I am {p2.name} and I am {p2.age} years old.")

p1 = person("aswin", 25)
p2 = person("Rajat", 20)

p1.introduce()
p2.introduce()
# introduce()

# print(p1.introduce())
# print(p2.introduce())
```

    Hi, I am aswin and I am 25 years old.
    Hi, I am Rajat and I am 20 years old.



```python
class product:
    def __init__(self, price):
        self.price = price

p = product(100)
del p.price

try:
    print(p.price)
    
except Exception as e:
    print("Error occurred:", e)


```

    Error occurred: 'product' object has no attribute 'price'



```python
class car:
    pass
    # def isinstance():
    #     pass
        
    # def type(self):
    #     pass

c = car()

print(isinstance(c,car))
print(type(c))
```

    True
    <class '__main__.car'>



```python
class car:
    pass

c = car()

print(isinstance(c, car))  # True
print(type(c))              # <class '__main__.User'>
```

    True
    <class '__main__.car'>



```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount

    def withdraw(self, amount):
        self.balance -= amount

BA = BankAccount("Aswin", balance = 50)

BA.deposit(2000)
BA.withdraw(500)

print(BA.balance)

    
```

    1550



```python

```


---
**Score: 10**