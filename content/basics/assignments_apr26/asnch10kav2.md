---
title: Asnch10Kav2
date: 2026-05-25
author: Your Name
cell_count: 7
score: 5
---

Chapter 10 – Python Date and Time
6. Write a Python program that prints the current date and time using the datetime
module. Format the output as: Day: DD, Month: MM, Year: YYYY, Time:
HH:MM:SS.
7. Using strftime(), convert the current datetime object into a string in the format:
Wednesday, 14 May 2025 – 03:45 PM.
8. Given the string '25-12-2024 08:30:00', use strptime() to parse it into a
datetime object and then print only the year and month from it.
9. Write a Python program that converts the Unix timestamp 1700000000 to a
human-readable datetime object, and then converts a datetime object back to a Unix
timestamp.
10. Using the time module, write a program that measures how long it takes to compute
the sum of all numbers from 1 to 1,000,000, and then makes the program pause for 2.5
seconds before printing the result.


```python
from datetime import datetime

# print(datetime.now())

dt = datetime.now()
# print(fdt)

fdt = dt.strftime("%d-%m-%Y %H:%M:%S")
print(fdt)
```

    16-05-2026 17:33:26



```python
fdt = dt.strftime("%A, %d %b %Y - %I:%M %p")
print(fdt)
```

    Saturday, 16 May 2026 - 05:33 PM



```python
from datetime import datetime
sdt = "25-12-2024 08:30:00"
dt = datetime.strptime(sdt, "%d-%m-%Y %H:%M:%S")
fsdt = dt.strftime("%Y %M")
print(fsdt)
```

    2024 30



```python
unix_ts = 1700000000
dt = datetime.fromtimestamp(unix_ts)
print("Unix time stamp:", unix_ts)
print("Human readable date:", dt)

dt_obj = datetime(2026, 5, 16, 14, 30, 0)
uts = dt_obj.timestamp()
print("Date and time", dt_obj)
print("Unix time stamp:", uts)
```

    Unix time stamp: 1700000000
    Human readable date: 2023-11-15 03:43:20
    Date and time 2026-05-16 14:30:00
    Unix time stamp: 1778922000.0



```python
import time

st = time.time()

total = sum(range(1, 100005))

et = time.time()

elapsedtime = et-st

time.sleep(2.5)

print(total)
print(elapsedtime)
```

    5000450010
    0.004216432571411133



```python

```


---
**Score: 5**