---
tags:
  - physics
  - advance
  - measurement
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Measurement and Scientific Method — การวัดและกระบวนการทางวิทยาศาสตร์

> *"Measure what is measurable, and make measurable what is not so."* — Galileo Galilei

Physics is fundamentally an experimental science, and every experiment begins with measurement. In this first topic of the ม.4 Physics (ว301) curriculum, students learn the foundations of scientific inquiry: how to pose questions, form hypotheses, design experiments, collect and analyse data, and communicate results. Equally important is the language of measurement — the International System of Units (SI), significant figures, dimensional analysis, and uncertainty — which together allow physicists to report results that are reproducible and meaningful.

This note covers the scientific method, SI base and derived units, unit conversion, significant figures, the rules for propagation of uncertainty, and dimensional analysis. These skills underpin every subsequent topic in mechanics and waves.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Scientific method, SI units, measurement, significant figures, error analysis, dimensional analysis | Use measuring instruments, record data with correct significant figures, estimate uncertainty, convert units, perform dimensional checks |
| **Semester 2** | (Reinforced through wave experiments) | Apply measurement skills in laboratory work on waves and oscillations |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| การวัด | Measurement | Comparison with a standard |
| ปริมาณ | Quantity | Physical quantity |
| หน่วย | Unit | Standard of measurement |
| หลักของหน่วย | Base unit | 7 SI base units |
| หน่วยอนุพันธ์ | Derived unit | e.g. N, J, W |
| ตัวเลขนัยสำคัญ | Significant figures | Precision indicator |
| ความไม่แน่นอน | Uncertainty | $\Delta x$ |
| ความคลาดเคลื่อน | Error | Systematic / random |
| การวิเคราะห์มิติ | Dimensional analysis | Checking homogeneity |
| สมมติฐาน | Hypothesis | Testable prediction |
| ทฤษฎี | Theory | Well-supported explanation |
| กฎ | Law | Concise, universal statement |

---

## 3 | Key Concepts

### 3.1 The Scientific Method

The scientific method is a systematic cycle of inquiry:

1. **Observation** — observe a phenomenon and ask a question
2. **Hypothesis** — propose a testable, falsifiable explanation
3. **Experiment** — design a controlled experiment (independent, dependent, control variables)
4. **Analysis** — collect data, process with statistics, plot graphs
5. **Conclusion** — accept, revise, or reject the hypothesis
6. **Communication** — publish so others can replicate

A **theory** is a well-substantiated explanation; a **law** is a concise description of a pattern (often mathematical) that holds across a wide range of conditions.

### 3.2 SI Base Units

| Quantity | Unit | Symbol |
|---|---|---|
| Length | metre | m |
| Mass | kilogram | kg |
| Time | second | s |
| Electric current | ampere | A |
| Temperature | kelvin | K |
| Amount of substance | mole | mol |
| Luminous intensity | candela | cd |

**Derived units** are built from base units, e.g.:

$$1\ \text{N} = 1\ \text{kg}\cdot\text{m}\cdot\text{s}^{-2}, \qquad 1\ \text{J} = 1\ \text{kg}\cdot\text{m}^2\cdot\text{s}^{-2}, \qquad 1\ \text{W} = 1\ \text{J}\cdot\text{s}^{-1}$$

### 3.3 Unit Conversion and Prefixes

| Prefix | Symbol | Factor |
|---|---|---|
| giga | G | $10^9$ |
| mega | M | $10^6$ |
| kilo | k | $10^3$ |
| centi | c | $10^{-2}$ |
| milli | m | $10^{-3}$ |
| micro | $\mu$ | $10^{-6}$ |
| nano | n | $10^{-9}$ |

Example: $5\ \text{km} = 5 \times 10^3\ \text{m} = 5000\ \text{m}$.

### 3.4 Significant Figures

Rules for counting significant figures:
- Non-zero digits are always significant
- Zeros between non-zero digits are significant
- Leading zeros are **not** significant
- Trailing zeros after a decimal point **are** significant

**Operations:**
- Addition/Subtraction: result limited by the term with fewest decimal places
- Multiplication/Division: result limited by the factor with fewest significant figures

Example: $2.50\ \text{cm} \times 3.4\ \text{cm} = 8.5\ \text{cm}^2$ (2 sig figs).

### 3.5 Uncertainty and Error

**Systematic error** (ความคลาดเคลื่อนเชิงเป็นระบบ) — consistent bias (e.g. zeroed incorrectly). Reduced by calibration.
**Random error** (ความคลาดเคลื่อนเชิงสุ่ม) — unpredictable fluctuations. Reduced by averaging.

For a measured value $x \pm \Delta x$, the **fractional uncertainty** is:

$$\frac{\Delta x}{x} \times 100\%$$

**Propagation rules** (for independent quantities):
- Sum/Difference: $\Delta q = \Delta a + \Delta b$
- Product/Quotient: $\frac{\Delta q}{q} = \frac{\Delta a}{a} + \frac{\Delta b}{b}$
- Power $q = a^n$: $\frac{\Delta q}{q} = |n|\frac{\Delta a}{a}$

### 3.6 Dimensional Analysis

Every physical equation must be **dimensionally homogeneous** — each term has the same dimensions. Using base dimensions M (mass), L (length), T (time):

- Velocity: $[v] = \text{L}\,\text{T}^{-1}$
- Acceleration: $[a] = \text{L}\,\text{T}^{-2}$
- Force: $[F] = \text{M}\,\text{L}\,\text{T}^{-2}$
- Energy: $[E] = \text{M}\,\text{L}^2\,\text{T}^{-2}$

Example — check $v = v_0 + at$:

$$[\text{L}\,\text{T}^{-1}] = [\text{L}\,\text{T}^{-1}] + [\text{L}\,\text{T}^{-2}][\text{T}] = [\text{L}\,\text{T}^{-1}]\ \checkmark$$

Dimensional analysis can validate a formula but cannot determine dimensionless constants.

---

## 4 | Common Problem Types

### Type 1: Unit conversion with prefixes
> Convert $0.045\ \text{MW}$ to watts.

**Solution:**
$$0.045\ \text{MW} = 0.045 \times 10^6\ \text{W} = 4.5 \times 10^4\ \text{W} = 45000\ \text{W}$$

### Type 2: Significant figures in a calculation
> Compute $a = 2.50\ \text{m} / 0.40\ \text{s}$ and round correctly.

**Solution:**
$$a = \frac{2.50}{0.40} = 6.25 \to 6.3\ \text{m/s}\ \text{(2 sig figs)}$$

### Type 3: Propagation of uncertainty
> A rectangle has sides $l = 5.0 \pm 0.1\ \text{cm}$ and $w = 3.0 \pm 0.1\ \text{cm}$. Find area with uncertainty.

**Solution:**
$$A = lw = 15\ \text{cm}^2, \qquad \frac{\Delta A}{A} = \frac{0.1}{5.0} + \frac{0.1}{3.0} = 0.0533$$
$$\Delta A = 15 \times 0.0533 \approx 0.8\ \text{cm}^2 \Rightarrow A = 15.0 \pm 0.8\ \text{cm}^2$$

### Type 4: Dimensional analysis check
> Is $v^2 = 2as$ dimensionally correct?

**Solution:**
$$[\text{L}^2\,\text{T}^{-2}] = [\text{L}\,\text{T}^{-2}][\text{L}] = [\text{L}^2\,\text{T}^{-2}]\ \checkmark$$

---

## 5 | Cross-Links

- [[02_Kinematics]] — measurement underpins all kinematic calculations
- [[03_Dynamics]] — SI units of force and mass first introduced here
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — scientific notation and algebra used throughout
