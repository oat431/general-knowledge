---
tags:
  - computer-science
  - advance
  - computational-thinking
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว331"]
---

# Computational Thinking — ความคิดเชิงคำนวณ

> *"Computational thinking is a fundamental skill for everyone, not just for computer scientists."* — Jeannette Wing

Computational thinking (ความคิดเชิงคำนวณ) is a problem-solving methodology that involves formulating problems and their solutions so that the solutions are represented in a form that can be effectively carried out by an information-processing agent. It is not about thinking like a computer, but rather about organising problems in ways that make them solvable through computation.

The IPST (สสวท.) curriculum introduces computational thinking in ม.4 (ว331) as the foundational mindset underlying all computer science study. It emphasises four core pillars — decomposition (การแบ่งแยก), pattern recognition (การจดจำรูปแบบ), abstraction (การสรุป/นามธรรม), and algorithm design (การออกแบบขั้นตอนวิธี) — applied to real-world problems before any programming begins.

---

## 1 | Course Coverage

### ม.4 (ว331)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Four pillars of computational thinking; problem decomposition; pattern recognition; abstraction; introduction to algorithms and pseudocode | Identify problems, break them into parts, recognise patterns, design simple algorithms |
| **Semester 2** | Flowchart design; real-world applications; translating algorithms to pseudocode; bridging CT to programming | Draw flowcharts, write pseudocode, evaluate solution correctness |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ความคิดเชิงคำนวณ | Computational Thinking | CT |
| การแบ่งแยก | Decomposition | Break down |
| การจดจำรูปแบบ | Pattern Recognition | Find trends |
| การสรุป/นามธรรม | Abstraction | Remove detail |
| ขั้นตอนวิธี | Algorithm | Step-by-step |
| รหัสเทียม | Pseudocode | Informal code |
| ผังงาน | Flowchart | Diagram |
| อัลกอริทึม | Algorithm | — |
| ปัญหาย่อย | Subproblem | From decomposition |
| ข้อมูลเข้า/ข้อมูลออก | Input / Output | I/O |

---

## 3 | Key Concepts

### 3.1 The Four Pillars of Computational Thinking

**Decomposition (การแบ่งแยก)** breaks a large, complex problem into smaller, manageable subproblems (ปัญหาย่อย). For example, building a website decomposes into designing the layout, writing content, coding HTML/CSS, and testing.

**Pattern Recognition (การจดจำรูปแบบ)** identifies similarities (ความคล้ายคลึง) among problems or within data. Recognising that a problem has been solved before lets us reuse a known solution.

**Abstraction (การสรุป/นามธรรม)** filters out irrelevant details and focuses on essential features. Driving a car requires knowing the steering wheel and pedals (essential), not the internal combustion physics (irrelevant detail).

**Algorithm Design (การออกแบบขั้นตอนวิธี)** develops a finite, ordered sequence of steps (ขั้นตอน) that produces the correct output for any valid input.

### 3.2 Flowcharts (ผังงาน)

Flowcharts are diagrams representing an algorithm using standard symbols:

| Symbol | Shape | Meaning |
|---|---|---|
| Terminator | Oval | Start / End (เริ่ม / สิ้นสุด) |
| Process | Rectangle | Action / computation |
| Decision | Diamond | Yes/No question (ใช่/ไม่ใช่) |
| Input/Output | Parallelogram | Data in or out |
| Flowline | Arrow | Direction of flow |

### 3.3 Pseudocode (รหัสเทียม)

Pseudocode (รหัสเทียม) is an informal, language-neutral description of an algorithm. It uses structural conventions of programming but omits strict syntax:

```
BEGIN
    READ score
    IF score >= 80 THEN
        PRINT "Grade A"
    ELSE
        PRINT "Try again"
    END IF
END
```

### 3.4 Problem-Solving Methodology

The general CT workflow:

1. **Understand** — define the problem and its inputs/outputs
2. **Decompose** — break into subproblems
3. **Recognise patterns** — find reusable structures
4. **Abstract** — generalise the solution
5. **Design algorithm** — write step-by-step pseudocode or flowchart
6. **Evaluate** — test with sample inputs and trace execution

---

## 4 | Common Problem Types

### Type 1: Decompose a Real-World Problem
> Break down the task "organise a school sports day" using decomposition.

**Solution:**

```
Organise Sports Day
├── Plan events and schedule
├── Prepare venue and equipment
├── Register participants
├── Assign referees and staff
├── Run the competition
└── Award prizes and cleanup
```

Each subproblem can be further decomposed — "Register participants" splits into announcement, form collection, and verification.

### Type 2: Find a Pattern and Generalise
> Given the sequence 2, 4, 6, 8, …, identify the pattern and write pseudocode for the nth term.

**Solution:**

Pattern: each term increases by 2 → even numbers → $a_n = 2n$.

```
BEGIN
    READ n
    result ← 2 * n
    PRINT result
END
```

```python
n = int(input("Enter n: "))
print(2 * n)
```

### Type 3: Draw a Flowchart for Finding the Maximum of Two Numbers

```
START
  ↓
READ a, b
  ↓
[ a > b ? ] ──No──→ PRINT b
  ↓ Yes
PRINT a
  ↓
END
```

---

## 5 | Cross-Links

- [[02_Data_Representation]] — how data is represented for computation
- [[04_Programming_Fundamentals]] — implementing algorithms in code
- [[06_Algorithms]] — formal algorithm design and analysis
- [[../../Advance/Mathematics/Fundamental/17_Sets|Mathematics: Sets]] — logical foundations
