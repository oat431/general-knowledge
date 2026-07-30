---
tags:
  - computer-science
  - advance
  - functions-modularity
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว332"]
---

# Functions and Modularity — ฟังก์ชันและโมดูล

> *"Functions are the primary tool for managing complexity in programming."* — adapted from Abelson & Sussman, SICP

Functions (ฟังก์ชัน) let programmers package a block of code under a name so it can be reused without rewriting it. Modularity (โมดูลาริตี) is the principle of building programs from small, self-contained units that communicate through well-defined inputs and outputs. The IPST curriculum introduces these in ม.5 (ว332) as the bridge between writing single scripts and building larger, maintainable programs.

Students learn to define functions with `def`, work with parameters (พารามิเตอร์) and return values (ค่าที่ส่งกลับ), understand variable scope (ขอบเขตของตัวแปร), write recursive (เรียกซ้ำ) functions, and import standard library modules (โมดูล) — the same techniques used in real software development.

---

## 1 | Course Coverage

### ม.5 (ว332)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Defining functions; parameters and arguments; return values; default and keyword arguments; variable scope | Write reusable functions, distinguish local/global scope |
| **Semester 2** | Recursion (base case, recursive case); importing modules; built-in functions; creating simple libraries | Implement recursion, use `math`/`random`, build a small module |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ฟังก์ชัน | Function | `def name():` |
| พารามิเตอร์ | Parameter | in definition |
| อาร์กิวเมนต์ | Argument | value passed |
| ค่าที่ส่งกลับ | Return value | `return x` |
| ค่าเริ่มต้น | Default argument | `def f(x=10)` |
| อาร์กิวเมนต์คีย์เวิร์ด | Keyword argument | `f(name="A")` |
| ขอบเขตของตัวแปร | Variable Scope | local / global |
| ตัวแปรเฉพาะที่ | Local variable | inside function |
| ตัวแปรส่วนกลาง | Global variable | outside, module-level |
| การเรียกซ้ำ | Recursion | function calls itself |
| กรณีฐาน | Base case | stops recursion |
| โมดูล | Module | `import math` |

---

## 3 | Key Concepts

### 3.1 Defining and Calling Functions

```python
def greet(name):              # parameter: name
    message = f"Hello, {name}!"
    return message            # return value

print(greet("Somchai"))       # argument: "Somchai"
```

A function with no explicit `return` returns `None`.

### 3.2 Parameters and Arguments

- **Positional arguments** — matched by order.
- **Keyword arguments** — matched by name, may be in any order.
- **Default arguments** — used when caller omits the value.

```python
def power(base, exponent=2):
    return base ** exponent

power(5)              # 25   (exponent defaults to 2)
power(2, 10)          # 1024 (positional)
power(base=3, exponent=4)  # 81 (keyword)
```

### 3.3 Return Values

A function returns **one** object, but it may be a tuple:

```python
def min_max(nums):
    return min(nums), max(nums)   # tuple

lo, hi = min_max([4, 1, 9, 2])
```

### 3.4 Variable Scope (ขอบเขตของตัวแปร)

- **Local scope (ตัวแปรเฉพาะที่)** — variables created inside a function; they vanish when the function ends.
- **Global scope (ตัวแปรส่วนกลาง)** — variables defined at module level; readable inside functions but need `global` to reassign.

```python
counter = 0              # global

def increment():
    global counter
    counter += 1

increment()
print(counter)           # 1
```

LEGB lookup order: **L**ocal → **E**nclosing → **G**lobal → **B**uilt-in.

### 3.5 Recursion (การเรียกซ้ำ)

A recursive function calls itself. Every recursion needs:

1. **Base case (กรณีฐาน)** — stops the recursion.
2. **Recursive case (กรณีเรียกซ้ำ)** — calls itself with a smaller problem.

```python
def factorial(n):
    if n <= 1:           # base case
        return 1
    return n * factorial(n - 1)   # recursive case

print(factorial(5))      # 120
```

**Caution:** missing or wrong base case → infinite recursion → `RecursionError`.

### 3.6 Built-in Functions

| Function | Purpose |
|---|---|
| `len(x)` | length of sequence |
| `range(n)` | generate 0..n-1 |
| `type(x)` | type of object |
| `abs(x)` | absolute value |
| `round(x, d)` | round to d decimals |
| `sum(iter)` | sum elements |
| `max / min` | largest / smallest |

### 3.7 Importing Modules (โมดูล)

```python
import math
print(math.sqrt(16))      # 4.0

from random import randint
print(randint(1, 6))      # dice roll 1–6

import datetime as dt
print(dt.date.today())
```

### 3.8 Creating a Simple Library

Save functions in `mymath.py`:

```python
# mymath.py
def circle_area(r):
    return 3.14159 * r ** 2

def is_prime(n):
    if n < 2: return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
```

Use it elsewhere:

```python
from mymath import circle_area, is_prime
print(circle_area(5))     # 78.53975
print(is_prime(17))       # True
```

---

## 4 | Common Problem Types

### Type 1: Temperature Converter Function
> Write a function `c_to_f(celsius)` that returns Fahrenheit.

```python
def c_to_f(celsius):
    return celsius * 9 / 5 + 32

print(c_to_f(100))        # 212.0
```

### Type 2: Fibonacci Recursion
> Return the nth Fibonacci number recursively.

```python
def fib(n):
    if n < 2:             # base case
        return n
    return fib(n - 1) + fib(n - 2)

print([fib(i) for i in range(8)])   # [0, 1, 1, 2, 3, 5, 8, 13]
```

### Type 3: Scope Question
> Predict the output.

```python
x = 10
def f():
    x = 5
    print(x)     # 5  (local)
f()
print(x)         # 10 (global unchanged)
```

### Type 4: Using a Module
> Roll two dice using `random`.

```python
from random import randint
def roll_two_dice():
    return randint(1, 6) + randint(1, 6)

print(roll_two_dice())    # 2–12
```

---

## 5 | Cross-Links

- [[04_Programming_Fundamentals]] — control structures used inside functions
- [[06_Algorithms]] — recursive algorithms (binary search, merge sort)
- [[01_Computational_Thinking]] — decomposition maps to modularity
- [[../../Advance/Mathematics/Fundamental/05_Functions|Mathematics: Functions]] — mathematical function concepts
