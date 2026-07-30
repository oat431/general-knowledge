---
tags:
  - chemistry
  - advance
  - kinetics
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Reaction Kinetics — จลนพลศาสตร์เคมี

> *"Thermodynamics tells you if a reaction can happen; kinetics tells you how fast."* — Anonymous

Reaction kinetics is the study of reaction rates and the molecular events that produce them. While thermodynamics (Topic 11) answers the question "Will it happen?", kinetics answers "How fast, and by what mechanism?" This topic is the second of three Semester 2 topics in ว312 and is essential for understanding catalysis, biological enzymes, industrial processes, and atmospheric chemistry.

This note covers the rate of reaction, the rate law, reaction order (zero, first, second), the rate constant, integrated rate laws, half-life, the Arrhenius equation, activation energy, collision theory, transition state theory, catalysis (homogeneous and heterogeneous), and reaction mechanisms including the rate-determining step.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Not covered — see Acids & Bases, Equilibrium) | — |
| **Semester 2** | Reaction rate, rate law, order of reaction (0, 1, 2), rate constant, integrated rate laws, half-life, Arrhenius equation, activation energy, catalysis, reaction mechanisms | Determine order from data, apply integrated rate laws, calculate $E_a$, identify rate-determining step, draw PE diagrams |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| จลนพลศาสตร์ | Kinetics | Study of reaction rates |
| อัตราการเกิดปฏิกิริยา | Reaction rate | $r$ (M/s) |
| กฎอัตรา | Rate law | $r = k[A]^m[B]^n$ |
| อันดับของปฏิกิริยา | Reaction order | Sum of exponents in rate law |
| ค่าคงที่อัตรา | Rate constant | $k$ |
| ปฏิกิริยาอันดับศูนย์ | Zero order | Rate independent of concentration |
| ปฏิกิริยาอันดับหนึ่ง | First order | Rate $\propto [A]$ |
| ปฏิกิริยาอันดับสอง | Second order | Rate $\propto [A]^2$ or $[A][B]$ |
| ครึ่งชีวิต | Half-life | $t_{1/2}$ |
| พลังงานกระตุ้น | Activation energy | $E_a$ (kJ/mol) |
| สมการอาเรนเนียส | Arrhenius equation | $k = A e^{-E_a/RT}$ |
| ทฤษฎีการชน | Collision theory | Frequency + orientation + $E$ |
| สถานะแทรนซิชัน | Transition state | Activated complex |
| ตัวเร่งปฏิกิริยา | Catalyst | Lowers $E_a$ |
| กลไกปฏิกิริยา | Reaction mechanism | Step-by-step pathway |
| ขั้นกำหนดอัตรา | Rate-determining step | Slowest step |
| สารมัธยันตร์ | Reaction intermediate | Formed and consumed |
| การเร่งปฏิกิริยาแบบเอกพันธ์ | Homogeneous catalysis | Same phase |
| การเร่งปฏิกิริยาแบบวิวิธพันธ์ | Heterogeneous catalysis | Different phase |
| แผนผังพลังงานศักย์ | PE diagram | Energy vs reaction progress |

---

## 3 | Key Concepts

### 3.1 Reaction Rate

Average rate: $r_{avg} = -\frac{\Delta [A]}{\Delta t}$ (with negative sign for reactants).
Instantaneous rate: $r = -\frac{d[A]}{dt} = \lim_{\Delta t \to 0} \frac{\Delta [A]}{\Delta t}$.

For $aA + bB \to cC + dD$:
$$r = -\frac{1}{a}\frac{d[A]}{dt} = -\frac{1}{b}\frac{d[B]}{dt} = \frac{1}{c}\frac{d[C]}{dt} = \frac{1}{d}\frac{d[D]}{dt}$$

### 3.2 The Rate Law

For a reaction $aA + bB \to \text{products}$:
$$r = k[A]^m[B]^n$$
$m$, $n$ are **reaction orders** with respect to each reactant; $m + n$ is the **overall order**. The exponents must be **determined experimentally** — they do not necessarily equal the stoichiometric coefficients.

### 3.3 Zero-Order Reactions

Rate is independent of concentration:
$$r = k \quad (\text{units of } k: \text{M/s})$$

Integrated law: $[A]_t = [A]_0 - kt$
Half-life: $t_{1/2} = \frac{[A]_0}{2k}$ (depends on initial concentration).
Example: surface-catalysed reactions where the surface is saturated.

### 3.4 First-Order Reactions

Rate proportional to one concentration:
$$r = k[A] \quad (k: \text{s}^{-1})$$

**Integrated rate law:**
$$\ln[A]_t = \ln[A]_0 - kt$$
or equivalently: $[A]_t = [A]_0 e^{-kt}$.

**Half-life:** $t_{1/2} = \frac{\ln 2}{k} = \frac{0.693}{k}$ (independent of $[A]_0$ — a hallmark of first order).
Examples: radioactive decay, many decomposition reactions, drug metabolism in the body.

### 3.5 Second-Order Reactions

Rate $\propto [A]^2$ or $[A][B]$:
$$r = k[A]^2 \quad (k: \text{M}^{-1}\text{s}^{-1})$$

**Integrated rate law:**
$$\frac{1}{[A]_t} = \frac{1}{[A]_0} + kt$$

**Half-life:** $t_{1/2} = \frac{1}{k[A]_0}$ (depends on initial concentration).

### 3.6 Determining Reaction Order Graphically

| Order | Plot that gives straight line | Slope |
|---|---|---|
| 0 | $[A]$ vs $t$ | $-k$ |
| 1 | $\ln[A]$ vs $t$ | $-k$ |
| 2 | $1/[A]$ vs $t$ | $+k$ |

If multiple reactants, use method of initial rates or pseudo-order conditions (flood one reactant).

### 3.7 Collision Theory

For a reaction to occur, molecules must:
1. **Collide** with sufficient frequency.
2. Have proper **orientation** (steric factor).
3. Possess kinetic energy ≥ $E_a$ (the activation energy).

This gives a rate constant proportional to collision frequency, fraction with $E \geq E_a$, and an orientation factor.

### 3.8 Transition State Theory

Reactants pass through a high-energy **transition state** (activated complex) before forming products. The PE diagram shows:
- Reactants → peak (transition state) → products
- $E_a$ = energy difference from reactants to peak (forward); or products to peak (reverse)
- $\Delta H$ = energy difference between reactants and products

### 3.9 Arrhenius Equation

$$k = A e^{-E_a / RT}$$
$$\ln k = \ln A - \frac{E_a}{R}\cdot\frac{1}{T}$$

A plot of $\ln k$ vs $1/T$ is a straight line with slope $-E_a/R$.

**Two-temperature form:**
$$\ln\frac{k_2}{k_1} = -\frac{E_a}{R}\left(\frac{1}{T_2} - \frac{1}{T_1}\right)$$

### 3.10 Catalysis

A catalyst provides an alternative pathway with lower $E_a$ (both forward and reverse are lowered equally; $\Delta H$ unchanged). It is not consumed.

- **Homogeneous**: same phase as reactants (e.g. $\ce{H+}$ catalysed ester hydrolysis in solution).
- **Heterogeneous**: different phase (e.g. solid Pt, Pd, or Ni in hydrogenation; catalytic converter in cars).
- **Enzymes** are biological catalysts — highly specific, work under mild conditions.

### 3.11 Reaction Mechanisms and the Rate Law

A mechanism is a sequence of elementary steps whose sum gives the overall reaction.
- **Elementary step**: the rate law is given directly by its molecularity (number of molecules colliding).
- **Rate-determining step (RDS)**: the slowest step; the rate law of the overall reaction matches the rate law of the RDS.
- **Reaction intermediates** are species produced in one step and consumed in another; they do **not** appear in the overall rate law.

For example:
$$\ce{2NO2 + F2 -> 2NO2F}$$
Proposed mechanism:
1. $\ce{NO2 + F2 -> NO2F + F}$ (slow, RDS)
2. $\ce{NO2 + F -> NO2F}$ (fast)

Rate law from RDS: $r = k[\ce{NO2}][\ce{F2}]$ — matches experiment.

---

## 4 | Common Problem Types

### Type 1: First-order integrated law
> A drug decomposes by first-order kinetics with $k = 0.025$ day⁻¹. If initial concentration is 1.0 × 10⁻³ M, what is it after 30 days?

**Solution:** $[\text{drug}]_t = [\text{drug}]_0 e^{-kt} = 1.0 \times 10^{-3} \times e^{-0.025 \times 30} = 1.0 \times 10^{-3} \times e^{-0.75}$
$= 1.0 \times 10^{-3} \times 0.472 = 4.72 \times 10^{-4}$ M.

### Type 2: First-order half-life
> Find the half-life of a first-order reaction with $k = 0.045$ s⁻¹.

**Solution:**
$$t_{1/2} = \frac{0.693}{k} = \frac{0.693}{0.045} = 15.4\ \text{s}$$

### Type 3: Determine order from data
> For reaction $A \to$ products:

| Time (s) | 0 | 20 | 40 | 60 | 80 |
|---|---|---|---|---|---|
| $[A]$ (M) | 1.00 | 0.82 | 0.67 | 0.55 | 0.45 |

Plot $\ln[A]$ vs $t$ → straight line. So **first order**.
Slope = $-k$. From data: slope ≈ $-0.010$ s⁻¹, so $k = 0.010$ s⁻¹.

### Type 4: Arrhenius — find $E_a$
> $k$ doubles when $T$ increases from 300 K to 310 K. Find $E_a$.

**Solution:**
$$\ln\frac{k_2}{k_1} = -\frac{E_a}{R}\left(\frac{1}{T_2} - \frac{1}{T_1}\right)$$
$$\ln 2 = -\frac{E_a}{8.314 \times 10^{-3}}\left(\frac{1}{310} - \frac{1}{300}\right)$$
$$0.693 = -\frac{E_a}{8.314 \times 10^{-3}} \times (-1.075 \times 10^{-4})$$
$$E_a = \frac{0.693 \times 8.314 \times 10^{-3}}{1.075 \times 10^{-4}} = 53.6\ \text{kJ/mol}$$

### Type 5: Mechanism analysis
> Mechanism: (1) $\ce{A2 <=> 2A}$ (fast equilibrium) (2) $\ce{A + B -> AB}$ (slow). What is the rate law?

**Solution:** Slow step: $r = k_2[\ce{A}][\ce{B}]$. From fast equilibrium: $K_1 = [\ce{A}]^2/[\ce{A2}]$, so $[\ce{A}] = \sqrt{K_1[\ce{A2}]}$.
$$r = k_2 \sqrt{K_1} \cdot [\ce{B}] \cdot \sqrt{[\ce{A2}]} = k_{eff}[\ce{B}][\ce{A2}]^{1/2}$$
Overall: order 3/2.

---

## 5 | Cross-Links

- [[05_Stoichiometry]] — mole ratios in rate expressions
- [[06_Solutions]] — concentration dependence
- [[07_Gases]] — collision theory (kinetic energy of gas molecules)
- [[09_Chemical_Equilibrium]] — equilibrium when forward = reverse rate
- [[11_Thermochemistry]] — PE diagrams, $\Delta H$ vs $E_a$, $\Delta G = -RT \ln K$
- [[13_Electrochemistry]] — Butler-Volmer equation; rate of electron transfer
- [[18_Biochemistry|Biology]] — enzyme kinetics (Michaelis-Menten)
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — logarithms, exponentials, differential equations
