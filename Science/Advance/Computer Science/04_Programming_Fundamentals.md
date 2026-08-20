---
tags:
  - computer-science
  - advance
  - programming-fundamentals
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว331"]
---

# Programming Fundamentals — พื้นฐานการเขียนโปรแกรม

> *"The most important property of a program is whether it accomplishes the intention of its user."* — C.A.R. Hoare

Programming fundamentals (พื้นฐานการเขียนโปรแกรม) are the building blocks every programmer must master before tackling larger problems. The IPST curriculum for ม.4 (ว331) uses Python as the teaching language and covers variables, data types, input/output, operators, and the three control structures (โครงสร้างควบคุม): sequence, selection (if/elif/else), and iteration (for, while).

By the end of the course students can write small programs that read input, compute results using arithmetic and logical operators, make decisions, repeat work with loops, and handle common errors through debugging (การดีบัก). These fundamentals underpin everything in ว332 — functions, modularity, and algorithm implementation.

---

## 1 | Course Coverage

### ม.4 (ว331)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Variables and naming; data types (int, float, str, bool); input/output; operators | Declare variables, use `print`/`input`, perform arithmetic |
| **Semester 2** | Control structures (if/elif/else, for, while); nested structures; common errors and debugging | Write branching and looping programs, trace and debug code |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ตัวแปร | Variable | named storage |
| ชนิดข้อมูล | Data Type | int, float, str, bool |
| จำนวนเต็ม | Integer (int) | whole numbers |
| จำนวนจริง | Float | decimals |
| สตริง/ข้อความ | String (str) | text |
| บูลีน | Boolean (bool) | True/False |
| ตัวดำเนินการ | Operator | +, -, *, == |
| โครงสร้างควบคุม | Control Structure | sequence/selection/iteration |
| การเลือก | Selection | if / elif / else |
| การทำซ้ำ | Iteration / Loop | for / while |
| การดีบัก | Debugging | find & fix errors |
| รหัสที่ซ้อนกัน | Nested structure | — |

---

## 3 | Key Concepts

### 3.1 Variables and Naming (ตัวแปร)

A variable is a named container for a value. Naming rules in Python:

- Must start with a letter or `_`; cannot start with a digit.
- Cannot be a keyword (`if`, `for`, `while`, …).
- Use descriptive `snake_case` names: `total_price`, not `tp`.

```python
age = 16            # int
pi = 3.14159        # float
name = "Somchai"    # str
is_student = True   # bool
```

### 3.2 Data Types (ชนิดข้อมูล)

| Type | Example | Notes |
|---|---|---|
| `int` (จำนวนเต็ม) | `42` | arbitrary precision in Python |
| `float` (จำนวนจริง) | `3.14` | 64-bit IEEE |
| `str` (ข้อความ) | `"hello"` | immutable sequence |
| `bool` (บูลีน) | `True` | subclass of int |

```python
x = int("15")      # string → int
y = str(15)        # int → string
z = float("2.5")   # string → float
```

### 3.3 Input and Output

```python
name = input("Enter your name: ")   # always returns str
age  = int(input("Enter your age: "))
print("Hello,", name, "you are", age)
```

Formatted (f-string) output:

```python
print(f"{name} is {age} years old")
```

### 3.4 Operators (ตัวดำเนินการ)

**Arithmetic:** `+  -  *  /  //  %  **`

```python
7 / 2    # 3.5   true division
7 // 2   # 3     floor division
7 % 2    # 1     modulo
2 ** 8   # 256   power
```

**Comparison:** `==  !=  >  <  >=  <=` → returns `bool`.

**Logical:** `and  or  not`.

**Assignment:** `=  +=  -=  *=  /=`.

```python
total = 0
total += 5      # total is now 5
total *= 2      # total is now 10
```

### 3.5 Control Structures (โครงสร้างควบคุม)

**Selection (การเลือก):**

```python
score = 75
if score >= 80:
    grade = "A"
elif score >= 70:
    grade = "B"
elif score >= 60:
    grade = "C"
else:
    grade = "F"
print(grade)   # B
```

**Iteration — `for` loop (การทำซ้ำแบบนับ):**

```python
for i in range(1, 6):       # 1,2,3,4,5
    print(i, "squared is", i*i)
```

**Iteration — `while` loop (การทำซ้ำแบบมีเงื่อนไข):**

```python
n = 10
while n > 0:
    print(n, end=" ")
    n -= 1
```

### 3.6 Nested Structures (โครงสร้างที่ซ้อนกัน)

Loops or conditionals placed inside one another. Multiplication table example:

```python
for i in range(1, 4):
    for j in range(1, 4):
        print(i * j, end="\t")
    print()
```

### 3.7 Common Errors and Debugging

| Error type | Thai | Example |
|---|---|---|
| Syntax error | ข้อผิดพลาดทางไวยากรณ์ | missing `:` after `if` |
| Name error | ข้อผิดพลาดชื่อ | using undefined variable |
| Type error | ข้อผิดพลาดชนิดข้อมูล | `"a" + 1` |
| Logic error | ข้อผิดพลาดทางตรรกะ | wrong formula, runs but wrong answer |

**Debugging tips:** read the traceback (การติดตามข้อผิดพลาด), use `print()` to inspect variables, test small pieces.

---

## 4 | Common Problem Types

### Type 1: Even or Odd
> Read an integer and print whether it is even (คู่) or odd (คี่).

```python
n = int(input("Enter a number: "))
if n % 2 == 0:
    print(n, "is even")
else:
    print(n, "is odd")
```

### Type 2: Sum 1 to N
> Compute the sum of integers from 1 to N.

```python
n = int(input("Enter N: "))
total = 0
for i in range(1, n + 1):
    total += i
print("Sum =", total)        # n*(n+1)//2
```

### Type 3: Factorial with `while`
> Compute $n!$ using a `while` loop.

```python
n = int(input("Enter n: "))
result, i = 1, 1
while i <= n:
    result *= i
    i += 1
print(f"{n}! = {result}")
```

### Type 4: Guess-the-Number Trace
> Predict the output of a nested loop before running.

```python
for i in range(3):           # i = 0,1,2
    for j in range(i + 1):   # grows each row
        print("*", end="")
    print()
# *
# **
# ***
```

---

## 5 | Cross-Links

- [[01_Computational_Thinking]] — algorithms become programs
- [[03_Boolean_Logic]] — conditions use Boolean expressions
- [[05_Functions_and_Modularity]] — packaging code into reusable units
- [[06_Algorithms]] — implementing searching & sorting
