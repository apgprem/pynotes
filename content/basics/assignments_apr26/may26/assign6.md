---
title: Assign6
date: 2026-06-26
author: Your Name
cell_count: 10
score: 10
---

ssignment 6: Temperature Tracker (Min, Max, Average)
Topics covered: Iteration, built-in functions, slicing
Task: A weather station recorded daily temperatures (in °C) for a week.
pythontemperatures = [22, 25, 19, 30, 28, 21, 24]

Print the highest and lowest temperature using max() and min().
Calculate and print the average temperature using sum() and len().
Print the temperatures of the first 3 days (weekdays start) using slicing.
Print the temperatures of the weekend (last 2 days) using negative slicing.
Use a for loop to print each day's temperature with a label like "Day 1: 22°C".
Use a list comprehension to create hot_days containing only temperatures above 25.


```python
pythontemperatures = [22, 25, 19, 30, 28, 21, 24]
# pythontemperatures.min()
print(min(pythontemperatures))
print(max(pythontemperatures))
```

    19
    30



```python
sum_list = sum(pythontemperatures)
len_list = len(pythontemperatures)

avg = sum_list/len_list

print(avg)
```

    24.142857142857142



```python
print("Temp of first 3 days", pythontemperatures[:3])
```

    Temp of first 3 days [22, 25, 19]



```python
print("Temp of last 2 days", pythontemperatures[-2:])
```

    Temp of last 2 days [21, 24]



```python
for index, temp in enumerate(pythontemperatures):
    print(f"Day {index}: {temp}°C")
```

    Day 0: 22°C
    Day 1: 25°C
    Day 2: 19°C
    Day 3: 30°C
    Day 4: 28°C
    Day 5: 21°C
    Day 6: 24°C



```python
for index, temp in enumerate(pythontemperatures, start=1):
    print(f"Day {index}: {temp}°C")
```

    Day 1: 22°C
    Day 2: 25°C
    Day 3: 19°C
    Day 4: 30°C
    Day 5: 28°C
    Day 6: 21°C
    Day 7: 24°C



```python
for index, temp in (pythontemperatures):
    print(f"Day {index}: {temp}°C")
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[19], line 1
    ----> 1 for index, temp in (pythontemperatures):
          2     print(f"Day {index}: {temp}°C")


    TypeError: cannot unpack non-iterable int object



```python
for temp in pythontemperatures:
    if temp>25:
        print(f"{temp}°C")
```

    30°C
    28°C



```python

```


---
**Score: 10**