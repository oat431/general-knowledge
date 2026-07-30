---
tags:
  - mathematics
  - advance
  - sequences
  - series
  - induction
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Sequences and Series — ลำดับและอนุกรม

> *"A sequence is a journey step by step; a series is the sum of the journey."*

Sequences and series extend students' understanding of patterns to formal mathematical structures. This topic covers arithmetic and geometric sequences, sigma notation, partial sums, and introduces mathematical induction as a proof technique. These concepts are foundational for calculus (infinite series) and discrete mathematics.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Sequences | Definition; explicit and recursive formulas; arithmetic sequences; geometric sequences |
| **Semester 2** | Series | Partial sums; sigma notation; arithmetic series; geometric series |
| **Semester 2** | Infinite geometric series | Convergence; sum formula $S = \frac{a_1}{1-r}$ for $|r| < 1$ |
| **Semester 2** | Mathematical induction | Base case; inductive step; proving formulas and inequalities |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| ลำดับ | Sequence | $a_n$ or $\{a_n\}$ |
| อนุกรม | Series | $S_n$ or $\sum a_n$ |
| ลำดับเลขคณิต | Arithmetic sequence | Common difference $d$ |
| ลำดับเรขาคณิต | Geometric sequence | Common ratio $r$ |
| พจน์ทั่วไป | General term / explicit formula | $a_n$ |
| สูตรเวียนเกิด | Recursive formula | $a_n = f(a_{n-1})$ |
| ผลบวกบางส่วน | Partial sum | $S_n$ |
| สัญกรณ์ซิกมา | Sigma notation | $\sum_{i=1}^n a_i$ |
| อนุกรมอนันต์ | Infinite series | $\sum_{n=1}^\infty a_n$ |
| การอุปนัยทางคณิตศาสตร์ | Mathematical induction | Proof technique |

---

## 3 | Key Concepts

### 3.1 Arithmetic Sequences

**Definition:** A sequence where each term differs from the previous by a constant $d$ (common difference).

**Explicit formula:**
$$a_n = a_1 + (n-1)d$$

**Recursive formula:**
$$a_1 = a, \quad a_n = a_{n-1} + d$$

**Example:** $3, 7, 11, 15, ...$ has $a_1 = 3$, $d = 4$
$$a_n = 3 + (n-1)(4) = 4n - 1$$

### 3.2 Arithmetic Series

**Sum of first n terms:**
$$S_n = \frac{n}{2}(a_1 + a_n) = \frac{n}{2}[2a_1 + (n-1)d]$$

**Example:** Find the sum of $3 + 7 + 11 + ... + 39$.

$a_n = 4n - 1 = 39 \Rightarrow n = 10$
$$S_{10} = \frac{10}{2}(3 + 39) = 5(42) = 210$$

### 3.3 Geometric Sequences

**Definition:** A sequence where each term is multiplied by a constant $r$ (common ratio).

**Explicit formula:**
$$a_n = a_1 \cdot r^{n-1}$$

**Recursive formula:**
$$a_1 = a, \quad a_n = r \cdot a_{n-1}$$

**Example:** $2, 6, 18, 54, ...$ has $a_1 = 2$, $r = 3$
$$a_n = 2 \cdot 3^{n-1}$$

### 3.4 Geometric Series

**Sum of first n terms:**
$$S_n = a_1 \cdot \frac{1 - r^n}{1 - r} \quad (r \neq 1)$$

**Infinite geometric series (converges if $|r| < 1$):**
$$S = \frac{a_1}{1 - r}$$

**Example:** Find the sum of $4 + 2 + 1 + 0.5 + ...$

$a_1 = 4$, $r = 0.5$, $|r| < 1$
$$S = \frac{4}{1 - 0.5} = \frac{4}{0.5} = 8$$

### 3.5 Sigma Notation

$$\sum_{i=1}^n a_i = a_1 + a_2 + ... + a_n$$

**Properties:**
$$\sum_{i=1}^n (a_i + b_i) = \sum_{i=1}^n a_i + \sum_{i=1}^n b_i$$
$$\sum_{i=1}^n c \cdot a_i = c \sum_{i=1}^n a_i$$
$$\sum_{i=1}^n c = nc$$

**Useful formulas:**
$$\sum_{i=1}^n i = \frac{n(n+1)}{2}$$
$$\sum_{i=1}^n i^2 = \frac{n(n+1)(2n+1)}{6}$$
$$\sum_{i=1}^n i^3 = \left[\frac{n(n+1)}{2}\right]^2$$

### 3.6 Mathematical Induction

**Principle:** To prove a statement $P(n)$ for all $n \geq 1$:

**Step 1 (Base case):** Show $P(1)$ is true.

**Step 2 (Inductive step):** Assume $P(k)$ is true for some $k \geq 1$, then prove $P(k+1)$ is true.

**Conclusion:** By induction, $P(n)$ is true for all $n \geq 1$.

**Example:** Prove $1 + 2 + ... + n = \frac{n(n+1)}{2}$

**Base case ($n=1$):** $1 = \frac{1(2)}{2} = 1$ ✓

**Inductive step:** Assume $1 + 2 + ... + k = \frac{k(k+1)}{2}$

Show: $1 + 2 + ... + k + (k+1) = \frac{(k+1)(k+2)}{2}$

$$1 + 2 + ... + k + (k+1) = \frac{k(k+1)}{2} + (k+1)$$
$$= \frac{k(k+1) + 2(k+1)}{2} = \frac{(k+1)(k+2)}{2}$$ ✓

---

## 4 | Common Problem Types

### Type 1: Arithmetic Sequence Term
> Find the 20th term of $5, 9, 13, 17, ...$

**Solution:** $a_1 = 5$, $d = 4$
$a_{20} = 5 + (20-1)(4) = 5 + 76 = 81$

### Type 2: Arithmetic Series Sum
> Find the sum of the first 50 positive even numbers.

**Solution:** Sequence: $2, 4, 6, ..., 100$
$a_1 = 2$, $a_{50} = 100$
$S_{50} = \frac{50}{2}(2 + 100) = 25(102) = 2550$

### Type 3: Geometric Sequence Term
> Find the 8th term of $3, 6, 12, 24, ...$

**Solution:** $a_1 = 3$, $r = 2$
$a_8 = 3 \cdot 2^7 = 3 \cdot 128 = 384$

### Type 4: Geometric Series Sum
> Find the sum of $5 + 5(0.4) + 5(0.4)^2 + ...$ (infinite series).

**Solution:** $a_1 = 5$, $r = 0.4$, $|r| < 1$
$S = \frac{5}{1 - 0.4} = \frac{5}{0.6} = \frac{25}{3}$

### Type 5: Sigma Notation
> Evaluate $\sum_{i=1}^5 (2i + 1)$.

**Solution:** $(2(1)+1) + (2(2)+1) + ... + (2(5)+1) = 3 + 5 + 7 + 9 + 11 = 35$

### Type 6: Induction Proof
> Prove that $7^n - 1$ is divisible by 6 for all $n \geq 1$.

**Solution:** 
Base case ($n=1$): $7^1 - 1 = 6$, divisible by 6 ✓

Inductive step: Assume $7^k - 1 = 6m$ for some integer $m$.
$7^{k+1} - 1 = 7 \cdot 7^k - 1 = 7(6m + 1) - 1 = 42m + 7 - 1 = 42m + 6 = 6(7m + 1)$
Divisible by 6 ✓

---

## 5 | Cross-Links

- [[Fundamental/10_Patterns_and_Algebraic_Thinking]] — Pattern recognition foundation
- [[14_Limits_and_Continuity]] — Infinite series and limits
- [[06_Exponential_and_Logarithmic_Functions]] — Geometric growth
- [[20_Discrete_Mathematics]] — Recurrence relations
