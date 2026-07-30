---
tags:
  - mathematics
  - advance
  - systems
  - equations
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Systems of Equations — ระบบสมการ

> *"A single equation describes a constraint; a system of equations describes a world."*

Systems of equations extend algebraic problem-solving from single equations to multiple simultaneous constraints. Students learn to find solutions that satisfy all equations at once, using substitution, elimination, matrix methods, and graphical analysis. These techniques are fundamental to optimization, physics, economics, and engineering.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Linear systems (2 variables) | Substitution method; elimination method; graphical method; consistent/inconsistent/dependent systems |
| **Semester 1** | Linear systems (3 variables) | Extension of elimination; back-substitution; geometric interpretation (planes) |
| **Semester 2** | Nonlinear systems | Systems with quadratic equations; substitution with polynomials; graphical analysis |
| **Semester 2** | Applications | Word problems; mixture problems; distance-rate-time; supply-demand equilibrium |

---

## 2 | Key Terminology

| Thai | English | Notes |
|---|---|---|
| ระบบสมการ | System of equations | Multiple equations with common variables |
| สมการเชิงเส้น | Linear equation | $ax + by = c$ |
| สมการไม่เชิงเส้น | Nonlinear equation | Contains $x^2$, $xy$, etc. |
| การแทนค่า | Substitution | Solve one equation, substitute into another |
| การกำจัดตัวแปร | Elimination | Add/subtract equations to eliminate variables |
| ระบบสมการที่สอดคล้องกัน | Consistent system | Has at least one solution |
| ระบบสมการที่ไม่สอดคล้องกัน | Inconsistent system | No solution |
| ระบบสมการพึ่งพา | Dependent system | Infinitely many solutions |
| จุดตัด | Intersection point | Solution on graph |

---

## 3 | Key Concepts

### 3.1 Linear Systems in 2 Variables

**General form:**
$$\begin{cases} a_1 x + b_1 y = c_1 \\ a_2 x + b_2 y = c_2 \end{cases}$$

**Three possible outcomes:**

| Type | Geometry | Algebra | Determinant |
|---|---|---|---|
| Consistent (independent) | Lines intersect at one point | One unique solution | $D \neq 0$ |
| Inconsistent | Parallel lines | No solution | $D = 0$, $D_x$ or $D_y \neq 0$ |
| Dependent | Same line | Infinitely many solutions | $D = D_x = D_y = 0$ |

### 3.2 Substitution Method

**Step 1:** Solve one equation for one variable (e.g., $y$ in terms of $x$)

**Step 2:** Substitute into the other equation

**Step 3:** Solve for the remaining variable

**Step 4:** Back-substitute to find the other variable

**Example:**
$$\begin{cases} 2x + y = 7 \\ x - y = 2 \end{cases}$$

From equation 2: $y = x - 2$

Substitute into equation 1: $2x + (x - 2) = 7 \Rightarrow 3x = 9 \Rightarrow x = 3$

Back-substitute: $y = 3 - 2 = 1$

**Solution:** $(3, 1)$

### 3.3 Elimination Method

**Step 1:** Multiply equations to make coefficients of one variable equal (or opposite)

**Step 2:** Add or subtract equations to eliminate that variable

**Step 3:** Solve for the remaining variable

**Step 4:** Back-substitute

**Example:**
$$\begin{cases} 3x + 2y = 12 \\ 5x - 2y = 4 \end{cases}$$

Add equations: $8x = 16 \Rightarrow x = 2$

Substitute: $3(2) + 2y = 12 \Rightarrow 6 + 2y = 12 \Rightarrow y = 3$

**Solution:** $(2, 3)$

### 3.4 Linear Systems in 3 Variables

**General form:**
$$\begin{cases} a_1 x + b_1 y + c_1 z = d_1 \\ a_2 x + b_2 y + c_2 z = d_2 \\ a_3 x + b_3 y + c_3 z = d_3 \end{cases}$$

**Strategy:** Eliminate one variable to reduce to a 2-variable system, then solve.

**Example:**
$$\begin{cases} x + y + z = 6 \\ 2x - y + z = 3 \\ x + 2y - z = 2 \end{cases}$$

Add equations 1 and 3: $2x + 3y = 8$ (eliminates z)

Add equations 2 and 3: $3x + y = 5$ (eliminates z)

Solve the 2×2 system: $x = 1, y = 2$

Back-substitute: $z = 3$

**Solution:** $(1, 2, 3)$

### 3.5 Nonlinear Systems

**Example:**
$$\begin{cases} x^2 + y^2 = 25 \\ x + y = 7 \end{cases}$$

From equation 2: $y = 7 - x$

Substitute: $x^2 + (7-x)^2 = 25$
$$x^2 + 49 - 14x + x^2 = 25$$
$$2x^2 - 14x + 24 = 0$$
$$x^2 - 7x + 12 = 0$$
$$(x-3)(x-4) = 0$$

So $x = 3$ or $x = 4$.

If $x = 3$, $y = 4$. If $x = 4$, $y = 3$.

**Solutions:** $(3, 4)$ and $(4, 3)$

---

## 4 | Common Problem Types

### Type 1: Linear System (Substitution)
> Solve: $\begin{cases} y = 2x + 1 \\ 3x - y = 5 \end{cases}$

**Solution:** Substitute $y$: $3x - (2x + 1) = 5 \Rightarrow x = 6, y = 13$

### Type 2: Linear System (Elimination)
> Solve: $\begin{cases} 4x + 3y = 11 \\ 4x - 3y = 5 \end{cases}$

**Solution:** Add: $8x = 16 \Rightarrow x = 2, y = 1$

### Type 3: Three-Variable System
> Solve: $\begin{cases} x + y + z = 10 \\ 2x - y = 3 \\ x + 2z = 8 \end{cases}$

**Solution:** From eq 2: $y = 2x - 3$. From eq 3: $z = 4 - x/2$.
Substitute into eq 1: $x + (2x-3) + (4-x/2) = 10 \Rightarrow x = 4, y = 5, z = 2$

### Type 4: Nonlinear System
> Solve: $\begin{cases} x^2 - y = 0 \\ x + y = 6 \end{cases}$

**Solution:** $y = 6 - x$, so $x^2 - (6-x) = 0 \Rightarrow x^2 + x - 6 = 0$
$(x+3)(x-2) = 0 \Rightarrow x = -3$ or $x = 2$
**Solutions:** $(-3, 9)$ and $(2, 4)$

### Type 5: Word Problem
> The sum of two numbers is 15. Their difference is 3. Find the numbers.

**Solution:** $x + y = 15$, $x - y = 3$. Add: $2x = 18 \Rightarrow x = 9, y = 6$

---

## 5 | Cross-Links

- [[Fundamental/11_Basic_Algebra]] — Linear equations foundation
- [[03_Algebraic_Expressions]] — Polynomial manipulation
- [[11_Matrices_and_Determinants]] — Matrix methods for systems
- [[05_Functions]] — Intersection of function graphs
