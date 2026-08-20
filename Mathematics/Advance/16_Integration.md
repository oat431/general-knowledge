---
tags:
  - mathematics
  - advance
  - integration
  - calculus
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค302"]
---

# Integration — การอินทิเกรต

> *"Integration is accumulation — adding up infinitely many infinitely small pieces."*

Integration is the reverse process of differentiation. This topic covers antiderivatives, definite and indefinite integrals, the Fundamental Theorem of Calculus, and techniques for evaluating integrals. Applications include finding area, volume, and total accumulation from rates of change.

---

## 1 | Course Coverage

### ม.5 (ค302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Antiderivatives | Reversing differentiation; basic integration rules |
| **Semester 2** | Indefinite integrals | $\int f(x)\,dx$; constant of integration $C$ |
| **Semester 2** | Definite integrals | $\int_a^b f(x)\,dx$; properties of definite integrals |
| **Semester 2** | Fundamental Theorem | Part 1 and Part 2; connecting derivatives and integrals |
| **Semester 2** | Integration techniques | Substitution (u-sub); integration by parts (intro) |
| **Semester 2** | Area applications | Area under curve; area between curves |
| **Semester 2** | Volume applications | Disk/washer method; shell method (intro) |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| ปริพันธ์ | Integral | $\int$ |
| อินทิเกรต | Integrate | Process |
| อินทิกรัลไม่ประจำ | Indefinite integral | $\int f(x)\,dx$ |
| อินทิกรัลประจำ | Definite integral | $\int_a^b f(x)\,dx$ |
| ค่าคงตัวของการอินทิเกรต | Constant of integration | $C$ |
| ฟังก์ชันปริพันธ์ | Antiderivative | $F(x)$ where $F'(x) = f(x)$ |
| ขอบเขต | Limits of integration | $a$ (lower), $b$ (upper) |
| ทฤษฎีบทมูลฐาน | Fundamental Theorem of Calculus | FTC |
| การเปลี่ยนตัวแปร | Substitution | $u$-substitution |
| พื้นที่ใต้กราฟ | Area under curve | $\int_a^b f(x)\,dx$ |

---

## 3 | Key Concepts

### 3.1 Antiderivatives

An **antiderivative** of $f(x)$ is a function $F(x)$ such that $F'(x) = f(x)$.

**General antiderivative:**
$$\int f(x)\,dx = F(x) + C$$

where $C$ is an arbitrary constant (since derivative of a constant is 0).

### 3.2 Basic Integration Rules

| Rule | Formula |
|---|---|
| Power rule ($n \neq -1$) | $\int x^n\,dx = \frac{x^{n+1}}{n+1} + C$ |
| Constant | $\int k\,dx = kx + C$ |
| Sum/Difference | $\int (f \pm g)\,dx = \int f\,dx \pm \int g\,dx$ |
| Constant multiple | $\int kf\,dx = k\int f\,dx$ |
| $1/x$ | $\int \frac{1}{x}\,dx = \ln|x| + C$ |
| Exponential | $\int e^x\,dx = e^x + C$ |
| Sine | $\int \sin x\,dx = -\cos x + C$ |
| Cosine | $\int \cos x\,dx = \sin x + C$ |
| Sec² | $\int \sec^2 x\,dx = \tan x + C$ |

### 3.3 Definite Integrals

$$\int_a^b f(x)\,dx = F(b) - F(a)$$

**Properties:**
- $\int_a^b f(x)\,dx = -\int_b^a f(x)\,dx$
- $\int_a^a f(x)\,dx = 0$
- $\int_a^b [f(x) + g(x)]\,dx = \int_a^b f(x)\,dx + \int_a^b g(x)\,dx$
- $\int_a^b kf(x)\,dx = k\int_a^b f(x)\,dx$
- $\int_a^c f(x)\,dx = \int_a^b f(x)\,dx + \int_b^c f(x)\,dx$

### 3.4 Fundamental Theorem of Calculus

**Part 1:** If $F(x) = \int_a^x f(t)\,dt$, then $F'(x) = f(x)$.

**Part 2:** If $F$ is an antiderivative of $f$ on $[a, b]$, then $\int_a^b f(x)\,dx = F(b) - F(a)$.

### 3.5 Integration by Substitution

**Method:** Let $u = g(x)$, then $du = g'(x)\,dx$.

**Example:** $\int 2x\sqrt{x^2 + 1}\,dx$

Let $u = x^2 + 1$, $du = 2x\,dx$.
$$\int \sqrt{u}\,du = \frac{2}{3}u^{3/2} + C = \frac{2}{3}(x^2+1)^{3/2} + C$$

### 3.6 Area Between Curves

$$\text{Area} = \int_a^b |f(x) - g(x)|\,dx$$

where $f(x) \geq g(x)$ on $[a, b]$ (top minus bottom).

**Example:** Find area between $y = x^2$ and $y = x$ on $[0, 1]$.

Intersect at $x = 0$ and $x = 1$. On this interval, $x \geq x^2$.
$$\int_0^1 (x - x^2)\,dx = \left[\frac{x^2}{2} - \frac{x^3}{3}\right]_0^1 = \frac{1}{2} - \frac{1}{3} = \frac{1}{6}$$

### 3.7 Volume by Disk Method

Revolving $y = f(x)$ about the x-axis:
$$V = \pi\int_a^b [f(x)]^2\,dx$$

**Example:** Find volume of solid formed by revolving $y = \sqrt{x}$ from $0$ to $4$ about x-axis.
$$V = \pi\int_0^4 x\,dx = \pi\left[\frac{x^2}{2}\right]_0^4 = 8\pi$$

### 3.8 Volume by Washer Method

When there is a gap between the curve and the axis of revolution:
$$V = \pi\int_a^b \left([R(x)]^2 - [r(x)]^2\right)\,dx$$

where $R(x)$ is the outer radius and $r(x)$ is the inner radius.

### 3.9 Average Value of a Function

$$f_{\text{avg}} = \frac{1}{b-a}\int_a^b f(x)\,dx$$

### 3.10 Integration by Parts (Intro)

$$\int u\,dv = uv - \int v\,du$$

**LIATE rule** for choosing $u$:
1. **L**ogarithmic ($\ln x$)
2. **I**nverse trig ($\sin^{-1} x$)
3. **A**lgebraic ($x^n$)
4. **T**rigonometric ($\sin x$)
5. **E**xponential ($e^x$)

Choose the type that appears **first** in LIATE as $u$.

**Example:** $\int x e^x\,dx$

Let $u = x$, $dv = e^x\,dx$. Then $du = dx$, $v = e^x$.
$$\int x e^x\,dx = xe^x - \int e^x\,dx = xe^x - e^x + C = e^x(x-1) + C$$

---

## 4 | Common Problem Types

### Type 1: Power Rule
> Evaluate $\int (6x^2 - 4x + 3)\,dx$.

**Solution:** $2x^3 - 2x^2 + 3x + C$

### Type 2: Definite Integral
> Evaluate $\int_1^3 (3x^2 + 2x)\,dx$.

**Solution:** $[x^3 + x^2]_1^3 = (27 + 9) - (1 + 1) = 34$

### Type 3: Substitution
> Evaluate $\int (3x^2 + 1)(x^3 + x)^4\,dx$.

**Solution:** Let $u = x^3 + x$, $du = (3x^2+1)\,dx$.
$\int u^4\,du = \frac{u^5}{5} + C = \frac{(x^3+x)^5}{5} + C$

### Type 4: Exponential
> Evaluate $\int e^{3x}\,dx$.

**Solution:** Let $u = 3x$, $du = 3\,dx$.
$\frac{1}{3}e^{3x} + C$

### Type 5: Area Between Curves
> Find the area enclosed between $y = x$ and $y = x^2$.

**Solution:** Intersection at $x = 0, 1$. Top function: $y = x$.
$\int_0^1 (x - x^2)\,dx = \frac{1}{2} - \frac{1}{3} = \frac{1}{6}$

### Type 6: Volume
> Find volume of solid formed by revolving $y = \sqrt{4-x^2}$ from $x = -2$ to $x = 2$ about x-axis.

**Solution:** $V = \pi\int_{-2}^2 (4-x^2)\,dx = \pi\left[4x - \frac{x^3}{3}\right]_{-2}^2$
$= \pi\left[\left(8-\frac{8}{3}\right) - \left(-8+\frac{8}{3}\right)\right] = \pi\cdot\frac{32}{3} = \frac{32\pi}{3}$

---

## 5 | Cross-Links

- [[15_Differentiation]] — Integration is reverse of differentiation
- [[14_Limits_and_Continuity]] — Integral defined via limits (Riemann sums)
- [[05_Functions]] — Area and volume from function graphs
- [[01_Physics - Overview]] — Work, displacement from velocity, center of mass
