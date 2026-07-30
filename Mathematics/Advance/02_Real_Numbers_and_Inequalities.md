---
tags:
  - mathematics
  - advance
  - real-numbers
  - inequalities
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Real Numbers and Inequalities — จำนวนจริงและอสมการ

> *"The real number line is the stage on which all of calculus performs."*

This topic formalizes the real number system and extends students' understanding of inequalities from simple linear cases to quadratic, rational, and absolute value inequalities. These skills are essential for determining domains, solving optimization problems, and understanding the behavior of functions.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Real number system review | Natural numbers (ℕ), integers (ℤ), rationals (ℚ), irrationals, reals (ℝ); field axioms; order properties |
| **Semester 1** | Absolute value | Definition; properties; equations \|ax + b\| = c; geometric interpretation as distance |
| **Semester 1** | Linear inequalities | ax + b < c; graphing on number line; interval notation |
| **Semester 1** | Quadratic inequalities | ax² + bx + c > 0; sign charts; test points |
| **Semester 1** | Rational inequalities | (ax + b)/(cx + d) ≥ 0; critical points; sign analysis |
| **Semester 2** | Absolute value inequalities | \|ax + b\| < c; \|ax + b\| > c; splitting into cases |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| จำนวนจริง | Real numbers | ℝ |
| จำนวนตรรกยะ | Rational numbers | ℚ |
| จำนวนอตรรกยะ | Irrational numbers | ℝ \ ℚ |
| จำนวนเต็ม | Integers | ℤ |
| จำนวนนับ | Natural numbers | ℕ |
| ค่าสัมบูรณ์ | Absolute value | \|x\| |
| อสมการ | Inequality | <, >, ≤, ≥ |
| ช่วง | Interval | (a, b), [a, b] |
| ช่วงเปิด | Open interval | (a, b) |
| ช่วงปิด | Closed interval | [a, b] |
| สัจพจน์ของฟิลด์ | Field axioms | — |
| สมบัติการเรียงลำดับ | Order properties | — |

---

## 3 | Key Concepts

### 3.1 Real Number System Hierarchy

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

**Irrational numbers:** Numbers that cannot be expressed as a/b where a, b ∈ ℤ, b ≠ 0.
Examples: $\sqrt{2}, \pi, e$

### 3.2 Absolute Value

**Definition:**
$$|x| = \begin{cases} x & \text{if } x \geq 0 \\ -x & \text{if } x < 0 \end{cases}$$

**Key properties:**
1. $|x| \geq 0$ for all $x \in \mathbb{R}$
2. $|x| = 0 \iff x = 0$
3. $|xy| = |x||y|$
4. $|x + y| \leq |x| + |y|$ (Triangle inequality)
5. $|x| = \sqrt{x^2}$

**Geometric interpretation:** $|x - a|$ is the distance between x and a on the number line.

### 3.3 Solving Absolute Value Equations

$$|ax + b| = c \text{ (where } c > 0)$$

**Split into two cases:**
$$ax + b = c \quad \text{or} \quad ax + b = -c$$

**Example:** $|2x - 3| = 5$
- Case 1: $2x - 3 = 5 \Rightarrow x = 4$
- Case 2: $2x - 3 = -5 \Rightarrow x = -1$

### 3.4 Interval Notation

| Inequality | Interval | Number Line |
|---|---|---|
| $a < x < b$ | $(a, b)$ | ○——○ |
| $a \leq x \leq b$ | $[a, b]$ | ●——● |
| $a \leq x < b$ | $[a, b)$ | ●——○ |
| $x > a$ | $(a, \infty)$ | ○→ |
| $x \geq a$ | $[a, \infty)$ | ●→ |

### 3.5 Solving Quadratic Inequalities

**Example:** $x^2 - 5x + 6 > 0$

**Step 1:** Find roots: $x^2 - 5x + 6 = (x-2)(x-3) = 0$
$$x = 2, \quad x = 3$$

**Step 2:** Create sign chart:

| Interval | Test Point | (x-2) | (x-3) | Product |
|---|---|---|---|---|
| $x < 2$ | x = 0 | − | − | + |
| $2 < x < 3$ | x = 2.5 | + | − | − |
| $x > 3$ | x = 4 | + | + | + |

**Step 3:** Solution (where product > 0):
$$x \in (-\infty, 2) \cup (3, \infty)$$

### 3.6 Solving Rational Inequalities

**Example:** $\frac{x-1}{x+2} \geq 0$

**Critical points:** Numerator = 0 at $x = 1$; Denominator = 0 at $x = -2$

**Sign chart:**

| Interval | Test Point | (x-1) | (x+2) | Quotient |
|---|---|---|---|---|
| $x < -2$ | x = -3 | − | − | + |
| $-2 < x < 1$ | x = 0 | − | + | − |
| $x > 1$ | x = 2 | + | + | + |

**Solution:** $x \in (-\infty, -2) \cup [1, \infty)$

> Note: $x = -2$ is excluded (makes denominator zero).

### 3.7 Absolute Value Inequalities

**Case 1:** $|x| < c$ (where $c > 0$)
$$-c < x < c$$

**Case 2:** $|x| > c$ (where $c > 0$)
$$x < -c \quad \text{or} \quad x > c$$

**Example:** $|2x - 3| < 5$
$$-5 < 2x - 3 < 5$$
$$-2 < 2x < 8$$
$$-1 < x < 4$$

---

## 4 | Common Problem Types

### Type 1: Absolute Value Equation
> Solve: $|3x + 2| = 7$

**Solution:**
- Case 1: $3x + 2 = 7 \Rightarrow x = \frac{5}{3}$
- Case 2: $3x + 2 = -7 \Rightarrow x = -3$

### Type 2: Quadratic Inequality
> Solve: $x^2 - 4x - 5 \leq 0$

**Solution:** Factor: $(x-5)(x+1) \leq 0$
Roots: $x = -1, 5$
Sign chart shows negative between roots.
**Answer:** $x \in [-1, 5]$

### Type 3: Rational Inequality
> Solve: $\frac{2x+1}{x-3} < 0$

**Solution:** Critical points: $x = -\frac{1}{2}, 3$
Sign chart shows negative in $(-\frac{1}{2}, 3)$.
**Answer:** $x \in (-\frac{1}{2}, 3)$

### Type 4: Absolute Value Inequality
> Solve: $|x - 4| \geq 2$

**Solution:**
- Case 1: $x - 4 \geq 2 \Rightarrow x \geq 6$
- Case 2: $x - 4 \leq -2 \Rightarrow x \leq 2$

**Answer:** $x \in (-\infty, 2] \cup [6, \infty)$

### Type 5: Nested Absolute Value
> Solve: $||x| - 3| = 2$

**Solution:**
$|x| - 3 = 2 \Rightarrow |x| = 5 \Rightarrow x = \pm 5$
$|x| - 3 = -2 \Rightarrow |x| = 1 \Rightarrow x = \pm 1$

**Answer:** $x \in \{-5, -1, 1, 5\}$

---

## 5 | Cross-Links

- [[Fundamental/01_Numbers_and_Numeration]] — Number system foundation
- [[Fundamental/07_Rational_Numbers]] — Rational vs irrational
- [[Fundamental/11_Basic_Algebra]] — Linear inequalities
- [[05_Functions]] — Domains defined by inequalities
- [[15_Differentiation]] — Finding critical points
