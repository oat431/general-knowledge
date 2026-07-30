---
tags: [overview, advanced-mathematics, discrete-math, proofs, linear-programming, high-school, ipst]
---

# Discrete and Advanced Topics — คณิตศาสตร์ไม่ต่อเนื่องและหัวข้อขั้นสูง

> **Category:** Advanced Mathematics (ม.4–ม.6, Sci-Math track)
> **Course:** ค303 (ม.6)
> **Covering:** Discrete Mathematics, Mathematical Reasoning/Proof, Linear Programming, Differential Equations

## Overview

The ม.6 curriculum brings together the most modern and applied branches of high school mathematics. Discrete mathematics equips students with tools for computer science. Mathematical reasoning teaches formal proof. Linear programming applies optimization to real-world problems. These topics represent the frontier of what Thai high school students encounter before university.

---

## Topic Areas

| # | Topic | Thai | Key Content |
|---|---|---|---|
| 20 | [[20_Discrete_Mathematics\|Discrete Mathematics]] | คณิตศาสตร์ไม่ต่อเนื่อง | Graph theory (vertices, edges, paths, trees), combinatorics, recurrence relations |
| 21 | [[21_Mathematical_Reasoning\|Mathematical Reasoning]] | การให้เหตุผลทางคณิตศาสตร์ | Direct proof, contradiction, contrapositive, mathematical induction |
| 22 | [[22_Linear_Programming\|Linear Programming]] | โปรแกรมเชิงเส้น | Optimization, constraints, feasible region, graphical method, simplex (intro) |
| 23 | [[23_Differential_Equations\|Differential Equations]] | สมการเชิงอนุพันธ์ | First-order ODEs, separation of variables, applications |

---

## Key Concepts

### Discrete Mathematics

| Topic | Description |
|---|---|
| **Graph Theory** | Vertices (nodes) connected by edges. Applications: networks, routing, social graphs |
| **Euler paths** | Path that uses every edge exactly once (bridges of Königsberg) |
| **Hamiltonian paths** | Path that visits every vertex exactly once (traveling salesman) |
| **Trees** | Connected acyclic graphs — n vertices have n−1 edges |
| **Combinatorics** | Counting techniques — permutations, combinations, pigeonhole principle |
| **Recurrence relations** | Fibonacci: Fₙ = Fₙ₋₁ + Fₙ₋₂, F₁ = F₂ = 1 |

### Mathematical Reasoning

| Proof Technique | Structure |
|---|---|
| **Direct proof** | Assume P, derive Q. P → Q |
| **Contrapositive** | Prove ¬Q → ¬P instead of P → Q |
| **Contradiction** | Assume ¬(P→Q), derive contradiction |
| **Mathematical induction** | Base case + inductive step: P(k) → P(k+1) |

**Classic proof:** √2 is irrational (by contradiction)

> Assume √2 = a/b (in lowest terms). Then 2 = a²/b², so a² = 2b². Thus a² is even, so a is even. Let a = 2k. Then 4k² = 2b², so b² = 2k². Thus b is also even. But then a/b is not in lowest terms — contradiction. ∴ √2 is irrational.

### Linear Programming

| Concept | Description |
|---|---|
| **Objective function** | The quantity to maximize or minimize (e.g., profit, cost) |
| **Constraints** | Inequalities defining the feasible region |
| **Feasible region** | Set of all points satisfying all constraints |
| **Corner point principle** | Optimal solution occurs at a vertex of the feasible region |
| **Graphical method** | Plot constraints, shade feasible region, test corner points |
| **Simplex method** | Systematic algorithm for high-dimensional LP problems |

### Differential Equations

| Type | Form | Solution Method |
|---|---|---|
| Separable | dy/dx = g(x)·h(y) | Separate variables, integrate both sides |
| Linear first-order | dy/dx + P(x)y = Q(x) | Integrating factor e^{∫P dx} |
| Applications | Population growth, radioactive decay, cooling | Model → ODE → solve → interpret |

---

## Key Thai Terminology

| Thai | English |
|---|---|
| ทฤษฎีกราฟ | Graph theory |
| จุดยอด / เส้นเชื่อม | Vertex / Edge |
| ต้นไม้ (ในทฤษฎีกราฟ) | Tree |
| การพิสูจน์ | Proof |
| ข้อขัดแย้ง | Contradiction |
| อุปนัยเชิงคณิตศาสตร์ | Mathematical induction |
| กำหนดการเชิงเส้น | Linear programming |
| ฟังก์ชันวัตถุประสงค์ | Objective function |
| อาณาบริเวณที่เป็นไปได้ | Feasible region |

---

## Exam Relevance

| Exam | Topics |
|---|---|
| **A-Level Math 1** | ~10-15% — Discrete math, proofs, linear programming |
| **PAT1** | ~10% — Proof techniques, linear programming problems |

---

## Cross-Links

- [[01_Advance Mathematics (Sci-Math) - Overview|← Back to Advanced Mathematics]]
- [[06 Foundations and Functions|Foundations and Functions]] — Logic feeds into proof techniques
- [[07 Calculus|Calculus]] — Differential equations connect to integration
- [[08 Algebra and Geometry|Algebra and Geometry]] — Linear programming uses systems of inequalities
- **Computer Science** — Graph theory, combinatorics, and algorithms are CS fundamentals
