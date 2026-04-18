---
title: Ioop
date: 2026-04-18
author: Your Name
cell_count: 11
score: 10
---

```python
print("Hello, Python!")
print(100)
print(3.14)
```

    Hello, Python!
    100
    3.14



```python
name = "Alice"
age = 30

print(name, age)  
# Output: Alice 30
```

    Alice 30



```python
print("Python", "is", "powerful", sep=" - ", end="!")
# Output: Python - is - powerful!
```

    Python - is - powerful!


```python
name = "Bob"
score = 88

print(f"Student {name} scored {score} marks.")
# Output: Student Bob scored 88 marks.
```

    Student Bob scored 88 marks.



```python
product = "Laptop"
price = 1200

print("The price of {} is ${}".format(product, price))
# Output: The price of Laptop is $1200
```

    The price of Laptop is $1200



```python
item = "Book"
quantity = 5

print("You bought %d %s(s)." % (quantity, item))
# Output: You bought 5 Book(s).
```

    You bought 5 Book(s).



```python
name = input("Enter your name: ")
print("Hello,", name)
```

    Enter your name:  prem


    Hello, prem



```python
age = int(input("Enter your age: "))

print(f"You will be {age + 1} next year.")
```

    Enter your age:  42


    You will be 43 next year.



```python
numbers = input("Enter two numbers: ").split()

num1 = int(numbers[0])
num2 = int(numbers[1])

print(num1 + num2)
```

    Enter two numbers:  25 30


    55



```python
with open("output.txt", "w") as file:
    print("This text goes into the file.", file=file)

print("Data successfully written to output.txt")
```

    Data successfully written to output.txt



```python

```


---
**Score: 10**