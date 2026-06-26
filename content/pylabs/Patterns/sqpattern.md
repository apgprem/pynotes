---
title: Sqpattern
date: 2026-06-26
author: Your Name
cell_count: 9
score: 5
---

```python
n=int(input("enter No"))

for i in range(n):
    for j in range(n):
        print("*",end=" ")
    print("")
```

    enter No 3


    * * * 
    * * * 
    * * * 



```python
n=int(input("enter No"))

for i in range(n):
    print("*"*n)
```

    enter No 2


    **
    **



```python
def print_hollow_square(n):
# n=int(input("enter no"))

    for i in range(n):
        for j in range(n):
            if i==0 or i==n-1 or j==0 or j==n-1:
                print("*",end=" ")
            else:
                print(" ",end=" ")
        print()
print_hollow_square(5)
```

    * * * * * 
    *       * 
    *       * 
    *       * 
    * * * * * 



```python
# Trianngle - Pattern - method 1

n=int(input("enter No"))

for i in range(n):
    for j in range(i):
        print("*",end=" ")
    print("")
```

    enter No 5


    
    * 
    * * 
    * * * 
    * * * * 



```python
# Trianngle - Pattern - method 2

n=int(input("enter No"))

for i in range(n):
    print("*"*i)
```

    enter No 5


    
    *
    **
    ***
    ****



```python
# Hollow Trianngle - Pattern

n=int(input("enter No"))

for i in range(n):
    for j in range(i+1):
        if j==0 or i==n-1 or i==j:
            print("* ",end=" ")
        else:
            print("  ",end=" ")
    print(" ")
```

    enter No 5


    *   
    *  *   
    *     *   
    *        *   
    *  *  *  *  *   



```python
# Right Trianngle - Pattern

n=int(input("enter No"))

for i in range(n,0,-1):
    for j in range(i):
        print("*",end=" ")
    print(" ")
```

    enter No 5


    * * * * *  
    * * * *  
    * * *  
    * *  
    *  



```python
# Right Trianngle - Pattern

n=int(input("enter No"))

for i in range(n-2):
    for j in range(n):
        print("*",end=" ")
    print(" ")
    
```

    enter No 5


    * * * * *  
    * * * * *  
    * * * * *  



```python

```


---
**Score: 5**