---
title: Variable Assignment
date: 2026-06-26
author: Your Name
cell_count: 19
score: 15
---

```python
# Variable assignment
count = 1
price = 99.99
name = "Python"

print(count)   # Output: 10
print(price)   # Output: 99.99
print(name)    # Output: Python

```

    10
    99.99
    Python



```python
# 2. Multiple Variable Assignment

a, b, c = 1, 2, 3

print(a)  # Output: 1
print(b)  # Output: 2
print(c)  # Output: 3

```

    1
    2
    3



```python
# 3. Reassigning Variables

value = 100
print(value)  # Output: 100

value = "Reassigned"
print(value)  # Output: Reassigned

```

    100
    Reassigned



```python
# 4. Numeric Literals

integer_literal = 42
float_literal = 3.14
complex_literal = 2 + 3j

print(integer_literal)  # Output: 42
print(float_literal)    # Output: 3.14
print(complex_literal)  # Output: (2+3j)
```

    42
    3.14
    (2+3j)



```python
# 5. String Literals
single_quote = 'Hello'
double_quote = "World"
multi_line = """This is
a multi-line
string"""

print(single_quote)  
print(double_quote)  
print(multi_line)
```

    Hello
    World
    This is
    a multi-line
    string



```python
is_active = True
is_logged_in = False

print(is_active)      # Output: True
print(is_logged_in)   # Output: False
```

    True
    False



```python
# 7. Special Literal: None

result = None

if result is None:
    print("No value assigned yet")
```

    No value assigned yet



```python
# 8. Collection Literals

list_literal = [1, 2, 3]
tuple_literal = (4, 5, 6)
set_literal = {7, 8, 9}
dict_literal = {"a": 1, "b": 2}

print(list_literal)   # Output: [1, 2, 3]
print(tuple_literal)  # Output: (4, 5, 6)
print(set_literal)    # Output: {7, 8, 9}
print(dict_literal)   # Output: {'a': 1, 'b': 2}
```

    [1, 2, 3]
    (4, 5, 6)
    {8, 9, 7}
    {'a': 1, 'b': 2}



```python
# 9. Binary, Octal, and Hexadecimal Literals

binary = 0b1010
octal = 0o12
hexadecimal = 0xA

print(binary)       # Output: 10
print(octal)        # Output: 10
print(hexadecimal)  # Output: 10
```

    10
    10
    10



```python
# 10. Using Variables in Expressions

x = 5
y = 3

sum_result = x + y
product_result = x * y

print(sum_result)      # Output: 8
print(product_result)  # Output: 15
```

    8
    15



```python
print("Python", "is", "powerful", sep=" * ", end="!")
# Output: Python - is - powerful!
```

    Python * is * powerful!


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
age = int(input("Enter your age: "))

print(f"You will be {age + 5} next year.")
```

    Enter your age:  40


    You will be 45 next year.



```python
numbers = input("Enter two numbers: ").split()

num1 = int(numbers[0])
num2 = int(numbers[1])
num3 = int(numbers[2])

print(num1 + num2 + num3)

```

    Enter two numbers:  10 15 20


    45



```python
with open("output.txt", "w") as file:
    print("This text goes into the file.", file=file)

print("Data successfully written to output.txt")
```

    Data successfully written to output.txt



```python
a = 10
b = 3

print(a + b)   # Addition → 13
print(a - b)   # Subtraction → 7
print(a * b)   # Multiplication → 30
print(a / b)   # Division → 3.333...
print(a // b)  # Floor Division → 3
print(a % b)   # Modulus → 1
print(a ** b)  # Exponentiation → 1000
```

    13
    7
    30
    3.3333333333333335
    3
    1
    1000



```python
a = 10
b = 3

print(a + b)   # Addition → 13
print(a - b)   # Subtraction → 7
print(a * b)   # Multiplication → 30
print(a / b)   # Division → 3.333...
print(a // b)  # Floor Division → 3
print(a % b)   # Modulus → 1
print(a ** b)  # Exponentiation → 1000
```

    13
    7
    30
    3.3333333333333335
    3
    1
    1000



```python

```


---
**Score: 15**