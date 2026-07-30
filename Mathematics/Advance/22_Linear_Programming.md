---
tags:
  - mathematics
  - advance
  - linear-programming
  - optimization
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค303"]
---

# Linear Programming — กำหนดการเชิงเส้น

> *"Linear programming finds the best outcome subject to given constraints — optimization made rigorous."*

Linear programming optimizes a linear objective function subject to linear constraints. This topic covers graphical methods for two-variable problems, the concept of feasible regions, and introduces the simplex method. Applications span economics, manufacturing, logistics, and resource allocation.

---

## 1 | Course Coverage

### ม.6 (ค303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | LP fundamentals | Objective function; constraints; feasible region; optimal solution |
| **Semester 2** | Graphical method | Graphing constraints; finding corner points; testing objective |
| **Semester 2** | Maximization/Minimization | Finding max and min of objective function |
| **Semester 2** | Special cases | No feasible region; unbounded; multiple optimal solutions |
| **Semester 2** | Simplex method (intro) | Standard form; pivoting; tableau |
| **Semester 2** | Applications | Resource allocation; diet problems; production planning |

---

## 2 | Key Terminology

| Thai | English | Notes |
|---|---|---|
| ฟังก์ชันเป้าหมาย | Objective function | Maximize or minimize $Z = ax + by$ |
| เงื่อนไขบังคับ | Constraints | Linear inequalities |
| ขอบเขตที่เป็นไปได้ | Feasible region | Region satisfying all constraints |
| จุดมุม | Corner point | Vertex of feasible region |
| คำตอบที่เหมาะสมที่สุด | Optimal solution | Max/min of objective |
| วิธีกำหนดการเชิงเส้น | Linear programming | LP |
| วิธีซิมเพล็กซ์ | Simplex method | Algebraic method for many variables |

---

## 3 | Key Concepts

### 3.1 Components of an LP Problem

**Standard form:**
$$	ext{Maximize (or minimize)} quad Z = c_1 x_1 + c_2 x_2 + ... + c_n x_n$$
$$	ext{Subject to:} quad a_{i1}x_1 + a_{i2}x_2 + ... + a_{in}x_n eq b_i$$
$$x_1, x_2, ..., x_n geq 0$$

### 3.2 Graphical Method (2 Variables)

**Steps:**
1. Graph each constraint as an equation (line)
2. Shade the feasible region (satisfies all inequalities)
3. Find corner points (vertices) of the feasible region
4. Evaluate objective function $Z$ at each corner point
5. Choose the maximum (or minimum) value

### 3.3 Corner Point Theorem

> If an optimal solution exists, it occurs at a corner point of the feasible region.

### 3.4 Example

**Problem:** Maximize $Z = 3x + 2y$ subject to:
$$x + y eq 4, quad 2x + y eq 6, quad x geq 0, quad y geq 0$$

**Step 1:** Find corner points of the feasible region.

| Constraint pair | Intersection |
|---|---|
| $x = 0$ and $y = 0$ | $(0, 0)$ |
| $x = 0$ and $x + y = 4$ | $(0, 4)$ |
| $x + y = 4$ and $2x + y = 6$ | $(2, 2)$ |
| $2x + y = 6$ and $y = 0$ | $(3, 0)$ |

**Step 2:** Evaluate $Z = 3x + 2y$ at each corner:

| Corner point | $Z = 3x + 2y$ |
|---|---|
| $(0, 0)$ | $0$ |
| $(0, 4)$ | $8$ |
| $(2, 2)$ | $10$ |
| $(3, 0)$ | $9$ |

**Optimal:** Maximum $Z = 10$ at $(2, 2)$.

### 3.5 Special Cases

| Case | Description |
|---|---|
| **No feasible region** | Constraints conflict; no solution |
| **Unbounded** | Feasible region extends infinitely; may not have max/min |
| **Multiple optimal** | Objective parallel to a constraint; infinitely many optima |
| **Degenerate** | Three or more constraints meet at one corner |

---

## 4 | Common Problem Types

### Type 1: Graphical Solution
> Maximize $Z = 5x + 3y$ subject to $x + y eq 6$, $2x + y eq 10$, $x, y geq 0$.

**Solution:** Corners: $(0,0)$, $(5,0)$, $(4,2)$, $(0,6)$
$Z$ values: $0, 25, 26, 18$
**Maximum: $Z = 26$ at $(4, 2)$**

### Type 2: Minimization
> Minimize $Z = 4x + 5y$ subject to $x + 2y geq 8$, $3x + y geq 9$, $x, y geq 0$.

**Solution:** Corners: $(0,9)$, $(2,3)$, $(8,0)$
$Z$ values: $45, 23, 32$
**Minimum: $Z = 23$ at $(2, 3)$**

### Type 3: Word Problem — Production
> A factory makes product A ($x$ units, profit 300 baht/unit) and product B ($y$ units, profit 200 baht/unit). Each unit of A requires 2 hours of machine time and 1 hour of labor. Each unit of B requires 1 hour of machine time and 2 hours of labor. Available: 8 machine hours, 8 labor hours. Find optimal production.

**Solution:**

Maximize $Z = 300x + 200y$ subject to:
$$2x + y \leq 8 \quad 	ext{(machine)}, \quad x + 2y \leq 8 \quad 	ext{(labor)}, \quad x, y \geq 0$$

**Corner points:**

| Constraint pair | Intersection |
|---|---|
| $x = 0, y = 0$ | $(0, 0)$ |
| $x = 0, x + 2y = 8$ | $(0, 4)$ |
| $2x + y = 8, x + 2y = 8$ | $(8/3, 8/3)$ |
| $2x + y = 8, y = 0$ | $(4, 0)$ |

**Evaluate $Z$:**

| Corner | $Z = 300x + 200y$ |
|---|---|
| $(0, 0)$ | $0$ |
| $(0, 4)$ | $800$ |
| $(8/3, 8/3)$ | $4000/3 \approx 1333$ |
| $(4, 0)$ | $1200$ |

**Optimal:** Produce $8/3 \approx 2.67$ units of each. If integer solutions required, test $(2, 3)$ and $(3, 2)$: $Z(2,3) = 1200$, $Z(3,2) = 1300$. So $x = 3, y = 2$ gives integer optimum $Z = 1300$ baht.

### Type 4: Word Problem — Diet (Minimization)
> Food X costs 4 baht/unit, Y costs 5 baht/unit. X provides 2 units of protein, Y provides 1 unit. X provides 1 unit of iron, Y provides 2 units. Minimum requirement: 8 units protein, 8 units iron. Find minimum cost.

**Solution:**

Minimize $C = 4x + 5y$ subject to:
$$2x + y \geq 8 \quad 	ext{(protein)}, \quad x + 2y \geq 8 \quad 	ext{(iron)}, \quad x, y \geq 0$$

**Corner points of feasible region (unbounded above):**

| Constraint pair | Intersection |
|---|---|
| $2x + y = 8, y = 0$ | $(4, 0)$ |
| $2x + y = 8, x + 2y = 8$ | $(8/3, 8/3)$ |
| $x + 2y = 8, x = 0$ | $(0, 4)$ |

**Evaluate $C$:**

| Corner | $C = 4x + 5y$ |
|---|---|
| $(4, 0)$ | $16$ |
| $(8/3, 8/3)$ | $72/3 = 24$ |
| $(0, 4)$ | $20$ |

**Optimal:** Buy 4 units of X, 0 units of Y. Minimum cost = 16 baht.

---

## 5 | Cross-Links

- [[04_Systems_of_Equations]] — Finding corner points
- [[11_Matrices_and_Determinants]] — Simplex method uses matrices
- [[12_Analytic_Geometry]] — Graphing constraints as lines
- [[02_Real_Numbers_and_Inequalities]] — Linear inequalities
