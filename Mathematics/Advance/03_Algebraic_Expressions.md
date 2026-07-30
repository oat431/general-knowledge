---
tags:
  - mathematics
  - advance
  - algebra
  - polynomials
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Algebraic Expressions — นิพจน์พีชคณิต

> *"Polynomials are the atoms of algebra — every expression is built from them."*

This topic deepens students' understanding of algebraic manipulation by focusing on polynomial operations, factoring techniques, and the fundamental theorems that govern polynomial behavior. These skills are essential for solving equations, simplifying expressions, and understanding function behavior.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Polynomial review | Monomials, binomials, trinomials; degree; leading coefficient; standard form |
| **Semester 1** | Polynomial operations | Addition, subtraction, multiplication; FOIL method; special products |
| **Semester 1** | Factoring techniques | GCF, difference of squares, perfect square trinomials, sum/difference of cubes, grouping |
| **Semester 1** | Remainder Theorem | Finding remainders without long division |
| **Semester 1** | Factor Theorem | Testing for factors; synthetic division |
| **Semester 1** | Polynomial division | Long division and synthetic division |

---

## 2 | Key Terminology

| Thai | English | Notes |
|---|---|---|
| พหุนาม | Polynomial | Sum of terms $a_n x^n + ... + a_1 x + a_0$ |
| เอกนาม | Monomial | Single term |
| ทวินาม | Binomial | Two terms |
|  trinomial | Trinomial | Three terms |
| ดีกรี | Degree | Highest power of x |
| สัมประสิทธิ์นำ | Leading coefficient | Coefficient of highest-degree term |
| การแยกตัวประกอบ | Factoring | Writing as product |
| ทฤษฎีบทเศษเหลือ | Remainder Theorem | $P(c)$ = remainder when dividing by $(x-c)$ |
| ทฤษฎีบทตัวประกอบ | Factor Theorem | $P(c) = 0 \iff (x-c)$ is a factor |
| การหารสังเคราะห์ | Synthetic division | Shortcut for dividing by $(x-c)$ |

---

## 3 | Key Concepts

### 3.1 Polynomial Standard Form

$$P(x) = a_n x^n + a_{n-1} x^{n-1} + ... + a_1 x + a_0$$

where $a_n \neq 0$, $n$ is the degree, and $a_n$ is the leading coefficient.

### 3.2 Special Product Formulas

**Difference of squares:**
$$(a + b)(a - b) = a^2 - b^2$$

**Perfect square trinomials:**
$$(a + b)^2 = a^2 + 2ab + b^2$$
$$(a - b)^2 = a^2 - 2ab + b^2$$

**Sum of cubes:**
$$(a + b)(a^2 - ab + b^2) = a^3 + b^3$$

**Difference of cubes:**
$$(a - b)(a^2 + ab + b^2) = a^3 - b^3$$

### 3.3 Factoring Strategies

**Step 1:** Factor out GCF (greatest common factor)

**Step 2:** Check for special patterns:
- Difference of squares: $a^2 - b^2 = (a+b)(a-b)$
- Perfect square trinomial: $a^2 \pm 2ab + b^2 = (a \pm b)^2$
- Sum/difference of cubes

**Step 3:** For trinomials $ax^2 + bx + c$:
- If $a = 1$: Find two numbers that multiply to $c$ and add to $b$
- If $a \neq 1$: Use AC method or grouping

**Step 4:** Factor by grouping (for 4+ terms)

### 3.4 Remainder Theorem

**Statement:** When polynomial $P(x)$ is divided by $(x - c)$, the remainder is $P(c)$.

**Example:** Find the remainder when $P(x) = 2x^3 - 5x^2 + 3x - 7$ is divided by $(x - 2)$.

**Solution:** $P(2) = 2(8) - 5(4) + 3(2) - 7 = 16 - 20 + 6 - 7 = -5$

### 3.5 Factor Theorem

**Statement:** $(x - c)$ is a factor of $P(x)$ if and only if $P(c) = 0$.

**Example:** Show that $(x - 1)$ is a factor of $P(x) = x^3 - 3x^2 + 4x - 2$.

**Solution:** $P(1) = 1 - 3 + 4 - 2 = 0$ ✓

### 3.6 Synthetic Division

**Example:** Divide $2x^3 - 5x^2 + 3x - 7$ by $(x - 2)$.

```
2 |  2   -5    3   -7
  |       4   -2    2
  -------------------
     2   -1    1   -5
```

**Result:** $2x^2 - x + 1$ with remainder $-5$

So: $\frac{2x^3 - 5x^2 + 3x - 7}{x - 2} = 2x^2 - x + 1 - \frac{5}{x - 2}$

### 3.7 Partial Fraction Decomposition

Breaking a rational expression into simpler fractions:

**Example:** $\frac{5x - 4}{x^2 - x - 2} = \frac{5x - 4}{(x-2)(x+1)}$

$$\frac{5x-4}{(x-2)(x+1)} = \frac{A}{x-2} + \frac{B}{x+1}$$

Multiply both sides by $(x-2)(x+1)$:
$$5x - 4 = A(x+1) + B(x-2)$$

Substitute $x = 2$: $10 - 4 = 3A \Rightarrow A = 2$

Substitute $x = -1$: $-5 - 4 = -3B \Rightarrow B = 3$

$$\frac{5x-4}{(x-2)(x+1)} = \frac{2}{x-2} + \frac{3}{x+1}$$

### 3.8 Rational Root Theorem

For polynomial $P(x) = a_n x^n + ... + a_0$ with integer coefficients:

Any rational root $\frac{p}{q}$ must have:
- $p$ dividing the constant term $a_0$
- $q$ dividing the leading coefficient $a_n$

**Example:** $P(x) = 2x^3 - 3x^2 - 11x + 6$

Possible rational roots: $\pm\{1, 2, 3, 6, 1/2, 3/2\}$

Test $x = 3$: $2(27) - 3(9) - 33 + 6 = 54 - 27 - 33 + 6 = 0$ ✓

So $(x - 3)$ is a factor. Divide to get $2x^2 + 3x - 2 = (2x - 1)(x + 2)$.

**All roots:** $x = 3, \frac{1}{2}, -2$

---

## 4 | Common Problem Types

### Type 1: Factoring Quadratics
> Factor: $x^2 - 7x + 12$

**Solution:** Find two numbers that multiply to 12 and add to -7: $-3$ and $-4$.
$$x^2 - 7x + 12 = (x - 3)(x - 4)$$

### Type 2: Factoring with GCF
> Factor: $6x^3 - 15x^2 + 9x$

**Solution:** GCF = $3x$
$$6x^3 - 15x^2 + 9x = 3x(2x^2 - 5x + 3) = 3x(2x - 3)(x - 1)$$

### Type 3: Difference of Squares
> Factor: $16x^2 - 25$

**Solution:** $(4x)^2 - 5^2 = (4x + 5)(4x - 5)$

### Type 4: Sum of Cubes
> Factor: $x^3 + 8$

**Solution:** $x^3 + 2^3 = (x + 2)(x^2 - 2x + 4)$

### Type 5: Using Remainder Theorem
> Find the remainder when $P(x) = x^4 - 3x^2 + 2x - 1$ is divided by $(x + 1)$.

**Solution:** $P(-1) = 1 - 3 - 2 - 1 = -5$

### Type 6: Using Factor Theorem
> Find a value of $k$ such that $(x - 2)$ is a factor of $P(x) = x^3 - kx^2 + 3x - 2$.

**Solution:** Set $P(2) = 0$:
$$8 - 4k + 6 - 2 = 0 \Rightarrow 12 - 4k = 0 \Rightarrow k = 3$$

---

## 5 | Cross-Links

- [[Fundamental/11_Basic_Algebra]] — Basic algebraic operations
- [[04_Systems_of_Equations]] — Solving systems using factoring
- [[05_Functions]] — Polynomial functions
- [[15_Differentiation]] — Derivatives of polynomials
