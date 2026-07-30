---
tags:
  - mathematics
  - advance
  - trigonometry
  - equations
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Trigonometric Equations — สมการตรีโกณมิติ

> *"Solving trig equations requires understanding both algebra and the periodic nature of trig functions."*

Trigonometric equations involve finding angles that satisfy equations containing trigonometric functions. This topic extends basic trig knowledge to solving complex equations using identities, factoring, and understanding the periodic nature of solutions. These skills are essential for physics, engineering, and signal processing.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Basic trig equations | $\sin\theta = a$, $\cos\theta = a$, $\tan\theta = a$; finding all solutions |
| **Semester 2** | Equations with identities | Using Pythagorean, double-angle, sum-to-product identities |
| **Semester 2** | Factoring trig equations | Factoring quadratic-like equations; zero product property |
| **Semester 2** | Multiple angles | Equations with $2\theta$, $3\theta$, etc.; adjusting solution intervals |
| **Semester 2** | Applications | Solving triangles; real-world periodic phenomena |

---

## 2 | Key Terminology

| Thai | English | Notes |
|---|---|---|
| สมการตรีโกณมิติ | Trigonometric equation | Contains trig functions |
| คำตอบทั่วไป | General solution | All solutions (with $+ 2n\pi$ or $+ n\pi$) |
| คำตอบเฉพาะ | Particular solution | Solutions in specific interval |
| คาบ | Period | Interval before function repeats |
| เอกลักษณ์ | Identity | True for all values |
| การแยกตัวประกอบ | Factoring | Writing as product |

---

## 3 | Key Concepts

### 3.1 Basic Equations

**$\sin\theta = a$** (where $|a| \leq 1$):
- Principal solution: $\theta = \sin^{-1}(a)$
- General solution: $\theta = \sin^{-1}(a) + 2n\pi$ or $\theta = \pi - \sin^{-1}(a) + 2n\pi$

**$\cos\theta = a$** (where $|a| \leq 1$):
- Principal solution: $\theta = \cos^{-1}(a)$
- General solution: $\theta = \cos^{-1}(a) + 2n\pi$ or $\theta = -\cos^{-1}(a) + 2n\pi$

**$\tan\theta = a$**:
- Principal solution: $\theta = \tan^{-1}(a)$
- General solution: $\theta = \tan^{-1}(a) + n\pi$

where $n$ is any integer.

### 3.2 Solving on Specific Intervals

**Example:** Solve $\sin\theta = \frac{1}{2}$ for $\theta \in [0, 2\pi)$.

$\sin^{-1}(1/2) = \pi/6$

Solutions in $[0, 2\pi)$:
- $\theta = \pi/6$ (Q1)
- $\theta = \pi - \pi/6 = 5\pi/6$ (Q2)

### 3.3 Using Identities

**Example:** Solve $2\sin^2\theta - \sin\theta - 1 = 0$ for $\theta \in [0, 2\pi)$.

Let $u = \sin\theta$: $2u^2 - u - 1 = 0$
$(2u + 1)(u - 1) = 0$

$u = -1/2$ or $u = 1$

$\sin\theta = -1/2 \Rightarrow \theta = 7\pi/6, 11\pi/6$
$\sin\theta = 1 \Rightarrow \theta = \pi/2$

**Solutions:** $\theta = \pi/2, 7\pi/6, 11\pi/6$

### 3.4 Factoring

**Example:** Solve $\sin\theta\cos\theta = 0$ for $\theta \in [0, 2\pi)$.

$\sin\theta = 0 \Rightarrow \theta = 0, \pi$
$\cos\theta = 0 \Rightarrow \theta = \pi/2, 3\pi/2$

**Solutions:** $\theta = 0, \pi/2, \pi, 3\pi/2$

### 3.5 Multiple Angles

**Example:** Solve $\sin(2\theta) = \frac{\sqrt{3}}{2}$ for $\theta \in [0, 2\pi)$.

Let $u = 2\theta$. Then $u \in [0, 4\pi)$.

$\sin u = \sqrt{3}/2 \Rightarrow u = \pi/3, 2\pi/3, 7\pi/3, 8\pi/3$

So $\theta = u/2$:
$\theta = \pi/6, \pi/3, 7\pi/6, 4\pi/3$

### 3.6 Double-Angle and Half-Angle Equations

**Example:** Solve $\cos(2\theta) = \cos\theta$ for $\theta \in [0, 2\pi)$.

Use identity: $\cos(2\theta) = 2\cos^2\theta - 1$

$2\cos^2\theta - 1 = \cos\theta$
$2\cos^2\theta - \cos\theta - 1 = 0$
$(2\cos\theta + 1)(\cos\theta - 1) = 0$

$\cos\theta = -1/2 \Rightarrow \theta = 2\pi/3, 4\pi/3$
$\cos\theta = 1 \Rightarrow \theta = 0$

**Solutions:** $\theta = 0, 2\pi/3, 4\pi/3$

### 3.7 Extraneous Solutions

When squaring both sides or using certain identities, extraneous solutions may appear. **Always check solutions in the original equation.**

---

## 4 | Common Problem Types

### Type 1: Basic Equation
> Solve $\cos\theta = -\frac{\sqrt{2}}{2}$ for $\theta \in [0, 2\pi)$.

**Solution:** $\cos^{-1}(-\sqrt{2}/2) = 3\pi/4$
Solutions: $\theta = 3\pi/4, 5\pi/4$

### Type 2: Quadratic Form
> Solve $2\cos^2\theta + \cos\theta - 1 = 0$ for $\theta \in [0, 2\pi)$.

**Solution:** $(2\cos\theta - 1)(\cos\theta + 1) = 0$
$\cos\theta = 1/2 \Rightarrow \theta = \pi/3, 5\pi/3$
$\cos\theta = -1 \Rightarrow \theta = \pi$
**Solutions:** $\pi/3, \pi, 5\pi/3$

### Type 3: Using Pythagorean Identity
> Solve $\sin^2\theta + \cos\theta = 1$ for $\theta \in [0, 2\pi)$.

**Solution:** Use $\sin^2\theta = 1 - \cos^2\theta$:
$1 - \cos^2\theta + \cos\theta = 1$
$-\cos^2\theta + \cos\theta = 0$
$\cos\theta(1 - \cos\theta) = 0$
$\cos\theta = 0 \Rightarrow \theta = \pi/2, 3\pi/2$
$\cos\theta = 1 \Rightarrow \theta = 0$
**Solutions:** $0, \pi/2, 3\pi/2$

### Type 4: Multiple Angle
> Solve $\tan(3\theta) = 1$ for $\theta \in [0, \pi)$.

**Solution:** $3\theta \in [0, 3\pi)$
$\tan(3\theta) = 1 \Rightarrow 3\theta = \pi/4, 5\pi/4, 9\pi/4$
$\theta = \pi/12, 5\pi/12, 3\pi/4$

### Type 5: Sum-to-Product
> Solve $\sin\theta + \sin(3\theta) = 0$ for $\theta \in [0, 2\pi)$.

**Solution:** Use sum-to-product: $\sin A + \sin B = 2\sin\left(\frac{A+B}{2}\right)\cos\left(\frac{A-B}{2}\right)$
$2\sin(2\theta)\cos(-\theta) = 0$
$2\sin(2\theta)\cos\theta = 0$
$\sin(2\theta) = 0$ or $\cos\theta = 0$
$2\theta = 0, \pi, 2\pi, 3\pi \Rightarrow \theta = 0, \pi/2, \pi, 3\pi/2$
$\cos\theta = 0 \Rightarrow \theta = \pi/2, 3\pi/2$
**Solutions:** $0, \pi/2, \pi, 3\pi/2$

---

## 5 | Cross-Links

- [[07_Trigonometric_Functions]] — Function properties and identities
- [[03_Algebraic_Expressions]] — Factoring techniques
- [[13_Vectors]] — Direction angles
- [[16_Integration]] — Trig integrals
