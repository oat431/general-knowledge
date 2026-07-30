---
tags:
  - computer-science
  - advance
  - boolean-logic
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว331"]
---

# Boolean Logic — ตรรกะแบบบูล

> *"The laws of thought, in their ultimate analysis, are the laws of combination of 0 and 1."* — George Boole

Boolean logic (ตรรกะแบบบูล) is the algebra of truth values — true (จริง) and false (เท็จ). Introduced by George Boole in 1854, it is the mathematical foundation of digital circuit design and of every conditional statement in programming. The IPST curriculum introduces it in ม.4 (ว331) alongside data representation, because binary values are naturally logical values.

Students learn the basic operations AND, OR, NOT (และ, หรือ, ไม่), extend to XOR, NAND, and NOR, build truth tables (ตารางค่าความจริง), apply De Morgan's laws to simplify expressions, and connect Boolean algebra to hardware logic gates (วงจรตรรกะ) and software `if` conditions.

---

## 1 | Course Coverage

### ม.4 (ว331)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Boolean values; AND/OR/NOT; truth tables; De Morgan's laws; logic gates | Build truth tables, simplify Boolean expressions |
| **Semester 2** | Boolean expressions in programming conditions; intro to XOR, NAND, NOR; applications | Translate logic to `if` statements and circuit symbols |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ตรรกะแบบบูล | Boolean Logic | Algebra of true/false |
| ค่าความจริง | Truth Value | True (1) / False (0) |
| ตารางค่าความจริง | Truth Table | All input combinations |
| ประพจน์ | Proposition | Statement with truth value |
| วงจรตรรกะ | Logic Gate / Circuit | Hardware |
| การพลิกค่า | Negation (NOT) | ¬A, !A |
| การเชื่อมแบบและ | Conjunction (AND) | A ∧ B |
| การเชื่อมแบบหรือ | Disjunction (OR) | A ∨ B |
| เอกซ์คลูซีฟออร์ | Exclusive OR (XOR) | A ⊕ B |
| กฎของเดอมอร์แกน | De Morgan's Laws | ¬(A∧B)=¬A∨¬B |

---

## 3 | Key Concepts

### 3.1 Boolean Values and Operations

A Boolean variable holds either **True (จริง, 1)** or **False (เท็จ, 0)**.

| Operation | Symbol | Returns True when… |
|---|---|---|
| AND (และ) | $A \wedge B$, `A and B` | both A and B are True |
| OR (หรือ) | $A \vee B$, `A or B` | at least one is True |
| NOT (ไม่) | $\neg A$, `not A` | A is False |
| XOR (เอกซ์คลูซีฟออร์) | $A \oplus B$, `A ^ B` | exactly one is True |
| NAND | $\overline{A \wedge B}$ | NOT of AND |
| NOR | $\overline{A \vee B}$ | NOT of OR |

### 3.2 Truth Tables (ตารางค่าความจริง)

A truth table lists every combination of inputs and the resulting output. For 2 variables there are $2^2 = 4$ rows; for 3 variables, $2^3 = 8$ rows.

| A | B | A∧B | A∨B | A⊕B | ¬A |
|---|---|-----|-----|-----|----|
| 0 | 0 | 0 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 | 1 | 0 |
| 1 | 1 | 1 | 1 | 0 | 0 |

### 3.3 Logic Gates (วงจรตรรกะ)

Logic gates are the hardware realisations of Boolean operations. NAND and NOR are **universal gates (เกตสากล)** — any Boolean function can be built from them alone.

| Gate | Symbol shape |
|---|---|
| AND | D-shape |
| OR | curved shield |
| NOT (inverter) | triangle + bubble |
| XOR | shield + extra curve |

### 3.4 De Morgan's Laws (กฎของเดอมอร์แกน)

Two transformation rules that "push" a negation through a conjunction/disjunction:

$$\neg(A \wedge B) \equiv \neg A \vee \neg B$$

$$\neg(A \vee B) \equiv \neg A \wedge \neg B$$

In Python: `not (a and b)` is equivalent to `(not a) or (not b)`.

### 3.5 Boolean Simplification

Using identities, expressions can be minimised:

| Identity | Form |
|---|---|
| Identity | $A \wedge 1 = A,\; A \vee 0 = A$ |
| Domination | $A \wedge 0 = 0,\; A \vee 1 = 1$ |
| Idempotent | $A \wedge A = A,\; A \vee A = A$ |
| Complement | $A \wedge \neg A = 0,\; A \vee \neg A = 1$ |
| Double negation | $\neg(\neg A) = A$ |

**Karnaugh maps (แผนผังคาร์นอ)** are a visual tool (introduced briefly) for simplifying expressions of up to 4 variables by grouping adjacent 1s.

### 3.6 Boolean Logic in Programming

```python
age = 18
has_id = True

if age >= 18 and has_id:
    print("Entry allowed")        # เข้าได้
else:
    print("Entry denied")         # ห้ามเข้า
```

Short-circuit evaluation (การประเมินแบบลัดวิธี): `A and B` skips B if A is False; `A or B` skips B if A is True.

---

## 4 | Common Problem Types

### Type 1: Build a Truth Table
> Construct the truth table for $F = (A \wedge B) \vee \neg C$.

**Solution:**

| A | B | C | A∧B | ¬C | F |
|---|---|---|-----|----|---|
| 0 | 0 | 0 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 0 | 1 | 1 |
| 1 | 0 | 0 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 | 1 | 1 |
| 1 | 1 | 1 | 1 | 0 | 1 |

### Type 2: Simplify Using De Morgan's Law
> Simplify `not (x > 0 and y > 0)`.

**Solution:** By De Morgan's law:

$$\neg(x>0 \wedge y>0) \equiv x \le 0 \vee y \le 0$$

```python
# equivalent forms
cond = not (x > 0 and y > 0)
cond = (x <= 0) or (y <= 0)
```

### Type 3: XOR Application
> Use XOR to detect whether an odd number of sensors are triggered.

```python
sensors = [True, False, True, True]
alarm = False
for s in sensors:
    alarm ^= s          # XOR accumulate
print(alarm)  # True → odd count triggered
```

---

## 5 | Cross-Links

- [[02_Data_Representation]] — binary 0/1 as logical false/true
- [[04_Programming_Fundamentals]] — `if` conditions use Boolean logic
- [[06_Algorithms]] — decision steps in algorithms
- [[../../Advance/Mathematics/Fundamental/17_Sets|Mathematics: Sets]] — set operations mirror Boolean algebra
