---
tags:
  - mathematics
  - advance
  - differential-equations
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค303"]
---

# Differential Equations — สมการเชิงอนุพันธ์

> *"Differential equations are the language of nature — Newton, Maxwell, and Schrödinger all spoke in this language."*

A differential equation relates a function to its derivatives. This topic introduces first-order ordinary differential equations (ODEs), methods for solving them, and applications to growth, decay, and mixing problems. Differential equations model virtually every physical system.

---

## 1 | Course Coverage

### ม.6 (ค303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | ODE basics | Definition; order; degree; general vs particular solution |
| **Semester 2** | Separable equations | Separating variables; integrating both sides |
| **Semester 2** | First-order linear | Integrating factor method; standard form |
| **Semester 2** | Initial value problems | Using initial conditions to find particular solution |
| **Semester 2** | Applications | Population growth; radioactive decay; Newton's law of cooling; mixing problems |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| สมการเชิงอนุพันธ์ | Differential equation | ODE |
| อันดับ | Order | Highest derivative |
| ระดับ | Degree | Power of highest derivative |
| คำตอบทั่วไป | General solution | Contains arbitrary constants |
| คำตอบเฉพาะ | Particular solution | Satisfies initial conditions |
| ปัญหาค่าเริ่มต้น | Initial value problem | IVP |
| การแยกตัวแปร | Separation of variables | Method |
| ตัวคูณอินทิเกรต | Integrating factor | $\mu(x)$ |

---

## 3 | Key Concepts

### 3.1 Definition and Classification

A **differential equation** is an equation involving an unknown function and its derivatives.

**Examples:**
- $\frac{dy}{dx} = 2x$ — First order, first degree
- $\frac{d^2y}{dx^2} + y = 0$ — Second order, first degree
- $(y')^2 + y = 0$ — First order, second degree

**Order:** The order of the highest derivative.

**Degree:** The power of the highest-order derivative (when the equation is polynomial in derivatives).

### 3.2 Separable Equations

A separable equation can be written:
$$\frac{dy}{dx} = g(x)h(y)$$

**Solution method:**
$$\frac{1}{h(y)}\,dy = g(x)\,dx$$
$$\int \frac{1}{h(y)}\,dy = \int g(x)\,dx + C$$

**Example:** Solve $\frac{dy}{dx} = xy$.

Separate: $\frac{dy}{y} = x\,dx$

Integrate: $\ln|y| = \frac{x^2}{2} + C_1$

Solve for $y$: $y = Ce^{x^2/2}$ (where $C = \pm e^{C_1}$)

### 3.3 First-Order Linear Equations

**Standard form:**
$$\frac{dy}{dx} + P(x)y = Q(x)$$

**Integrating factor:**
$$\mu(x) = e^{\int P(x)\,dx}$$

**Solution:**
$$y = \frac{1}{\mu(x)} \int \mu(x) Q(x)\,dx + \frac{C}{\mu(x)}$$

**Example:** Solve $y' + 2y = e^x$.

$P(x) = 2$, $Q(x) = e^x$

Integrating factor: $\mu = e^{\int 2\,dx} = e^{2x}$

Multiply: $e^{2x}y' + 2e^{2x}y = e^{2x} \cdot e^x = e^{3x}$

Left side is $(e^{2x}y)'$:
$(e^{2x}y)' = e^{3x}$

Integrate: $e^{2x}y = \frac{e^{3x}}{3} + C$

$$y = \frac{e^x}{3} + Ce^{-2x}$$

### 3.4 Initial Value Problems

Given a differential equation and an initial condition, find the particular solution.

**Example:** Solve $\frac{dy}{dx} = 2x$ with $y(0) = 3$.

Integrate: $y = x^2 + C$

Apply IC: $3 = 0 + C \Rightarrow C = 3$

**Particular solution:** $y = x^2 + 3$

### 3.5 Applications

**Exponential growth/decay:** $\frac{dP}{dt} = kP$

Solution: $P(t) = P_0 e^{kt}$

**Newton's Law of Cooling:** $\frac{dT}{dt} = -k(T - T_s)$

where $T_s$ is surrounding temperature.

Solution: $T(t) = T_s + (T_0 - T_s)e^{-kt}$

**Mixing problems:** Salt in a tank. If $Q(t)$ is the amount of salt:
$$\frac{dQ}{dt} = \text{rate in} - \text{rate out}$$

---

## 4 | Common Problem Types

### Type 1: Separation of Variables
> Solve $\frac{dy}{dx} = \frac{x}{y}$.

**Solution:** $y\,dy = x\,dx$
$\int y\,dy = \int x\,dx$
$\frac{y^2}{2} = \frac{x^2}{2} + C$
$y^2 = x^2 + C$

### Type 2: Growth/Decay
> A population grows at rate proportional to its size. Initial: 1000, after 2 hours: 3000. Find population at $t = 5$.

**Solution:** $P = P_0 e^{kt}$. $3000 = 1000e^{2k} \Rightarrow e^{2k} = 3 \Rightarrow k = \frac{\ln 3}{2}$
$P(5) = 1000e^{5\ln 3/2} = 1000 \cdot 3^{5/2} \approx 15,588$

### Type 3: First-Order Linear
> Solve $y' + \frac{1}{x}y = x$.

**Solution:** $P = 1/x$, $\mu = e^{\ln x} = x$
$(xy)' = x^2$
$xy = \frac{x^3}{3} + C$
$y = \frac{x^2}{3} + \frac{C}{x}$

### Type 4: Initial Value Problem
> Solve $y' = 3x^2$ with $y(1) = 5$.

**Solution:** $y = x^3 + C$. $5 = 1 + C \Rightarrow C = 4$.
$y = x^3 + 4$

### Type 5: Newton's Law of Cooling
> An object at 80°C in a room at 20°C cools to 50°C in 10 min. Find temperature at $t = 20$.

**Solution:** $T = 20 + 60e^{-kt}$. $50 = 20 + 60e^{-10k} \Rightarrow e^{-10k} = 0.5 \Rightarrow k = \frac{\ln 2}{10}$
$T(20) = 20 + 60e^{-2\ln 2} = 20 + 60(0.25) = 20 + 15 = 35°C$

### Type 6: Mixing Problem
> A tank has 100 L of water with 10 kg salt. Brine enters at 5 L/min with 0.2 kg/L salt. Mixed solution leaves at 5 L/min. Find salt amount at time $t$.

**Solution:** Rate in = $5(0.2) = 1$ kg/min. Rate out = $5 \cdot \frac{Q}{100} = \frac{Q}{20}$ kg/min.
$\frac{dQ}{dt} = 1 - \frac{Q}{20}$
This is first-order linear. $Q = 20 + Ce^{-t/20}$.
$Q(0) = 10 \Rightarrow 10 = 20 + C \Rightarrow C = -10$.
$Q(t) = 20 - 10e^{-t/20}$

---

## 5 | Cross-Links

- [[15_Differentiation]] — Derivatives in ODEs
- [[16_Integration]] — Solving ODEs requires integration
- [[14_Limits_and_Continuity]] — Solutions as functions
- [[06_Exponential_and_Logarithmic_Functions]] — Growth/decay solutions
- [[01_Physics - Overview]] — Newton's laws, circuits, mechanics
