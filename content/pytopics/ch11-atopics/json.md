---
title: Json
date: 2026-06-26
author: Your Name
cell_count: 12
score: 10
---

1. What is JSON

JSON (JavaScript Object Notation) is a lightweight data-interchange format used for storing and exchanging structured data.

{
  "name": "Alice",
  "age": 30,
  "active": true
}

In Python, JSON is handled using the built-in json module.

2. Importing the JSON Module

import json

Provides methods to convert between Python objects and JSON format.


```python
# 3. Convert Python Object → JSON String (json.dumps)

import json

data = {"name": "Alice", "age": 30, "city": "Toronto"}
json_string = json.dumps(data)

print(json_string)

# Serializes Python objects into a JSON-formatted string.
```

    {"name": "Alice", "age": 30, "city": "Toronto"}



```python
# 4. Convert JSON String → Python Object (json.loads)

import json

json_text = '{"name": "Bob", "age": 25}'
python_obj = json.loads(json_text)

print(python_obj)
print(type(python_obj))  # dict

# Deserializes JSON string into Python data structures.
```

    {'name': 'Bob', 'age': 25}
    <class 'dict'>



```python
# 5. Writing JSON to a File (json.dump)

import json

data = {
    "product": "Laptop",
    "price": 1200,
    "in_stock": True
}

with open("product.json", "w") as file:
    json.dump(data, file)

# Stores structured data persistently.
```


```python
# 6. Reading JSON from a File (json.load)
import json

with open("product.json", "r") as file:
    data = json.load(file)

print(data)

# Loads JSON data into Python objects.
```

    {'product': 'Laptop', 'price': 1200, 'in_stock': True}



```python
# 7. Pretty Printing JSON

import json

data = {"name": "Alice", "skills": ["Python", "AI", "ML"]}

pretty_json = json.dumps(data, indent=10)
print(pretty_json)
```

    {
              "name": "Alice",
              "skills": [
                        "Python",
                        "AI",
                        "ML"
              ]
    }



```python
# 8. Handling Complex Data Types

import json
from datetime import datetime

data = {"event": "login", "time": str(datetime.now())}

json_string = json.dumps(data)
print(json_string)

# Non-serializable objects must be converted manually.
```

    {"event": "login", "time": "2026-06-01 08:25:17.383924"}



```python
# 9. Sorting JSON Keys

import json

data = {"b": 2, "a": 1, "c": 3}
sorted_json = json.dumps(data, sort_keys=True)

print(sorted_json)

# Useful for consistent API responses and hashing.
```

    {"a": 1, "b": 2, "c": 3}



```python
# 10. Enterprise Example: API Response Handling

import json

def parse_api_response(response):
    try:
        data = json.loads(response)
        return data.get("status"), data.get("payload")
    except json.JSONDecodeError:
        return "error", None

response = '{"status": "success", "payload": {"id": 101}}'
print(parse_api_response(response))

# Standard pattern for microservices and REST APIs.
```

    ('success', {'id': 101})


Common JSON Errors
Error - Cause

JSONDecodeError - Invalid JSON syntax

TypeError - Non-serializable object

UnicodeDecodeError - Encoding mismatch

Best Practices

    Always validate JSON structure

    Use try-except for decoding

    Avoid storing sensitive data in plain JSON

    Format JSON for logs but compress for production

    Use schema validation (e.g., Pydantic, Marshmallow)


---
**Score: 10**