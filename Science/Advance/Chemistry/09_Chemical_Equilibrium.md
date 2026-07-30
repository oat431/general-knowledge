---
tags:
  - chemistry
  - advance
  - equilibrium
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Chemical Equilibrium — สมดุลเคมี

> *"A reversible reaction is a conversation between reactants and products — equilibrium is the moment neither has the last word."* — Adapted from thermodynamics

Most chemical reactions do not go to completion; they reach a state of **dynamic equilibrium** where the forward and reverse rates are equal. The study of chemical equilibrium explains why some reactions appear to "stop" before all reactants are consumed, and gives us the tools to predict how a system at equilibrium will respond to disturbance. This is the second of three equilibrium-flavoured topics in ว312.

This note covers reversible reactions, the equilibrium constants $K_c$ and $K_p$, the reaction quotient $Q$, Le Chatelier's principle, ICE (Initial–Change–Equilibrium) tables, heterogeneous equilibrium, and the relationship between equilibrium position and equilibrium constant.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Reversible reactions, $K_c$, $K_p$, Le Chatelier's principle (conc/pressure/temp), ICE tables, heterogeneous equilibrium, $Q$ vs $K$, effect of catalysts | Write equilibrium expressions, set up and solve ICE tables, predict shift direction, calculate $K_p$ from $K_c$ |
| **Semester 2** | (Not covered — see Thermochemistry, Kinetics, Electrochemistry) | — |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| สมดุลเคมี | Chemical equilibrium | Dynamic; rates equal |
| ปฏิกิริยาผันกลับ | Reversible reaction | Denoted $\rightleftharpoons$ |
| สมดุลพลวัต | Dynamic equilibrium | Forward = reverse rate |
| ค่าคงที่สมดุล | Equilibrium constant | $K_c$ (conc), $K_p$ (pressure) |
| ความเข้มข้น | Concentration | mol/L (M) |
| ความดันย่อย | Partial pressure | atm or bar |
| ตาราง ICE | ICE table | Initial, Change, Equilibrium |
| หลักเลอชาเทลิเย | Le Chatelier's principle | System opposes disturbance |
| สมดุลเอกพันธ์ | Homogeneous equilibrium | All species same phase |
| สมดุลวิวิธพันธ์ | Heterogeneous equilibrium | Mixed phases |
| ค่า Q (รีเอชันโควอชันต์) | Reaction quotient | Same form as $K$ |
| ตำแหน่งสมดุล | Equilibrium position | Actual concentrations |
| ค่าคงที่สมดุล | Equilibrium constant | Magnitude only (depends on $T$) |
| ตัวเร่งปฏิกิริยา | Catalyst | Speeds up both directions |
| อุณหภูมิ | Temperature | Only factor changing $K$ |

---

## 3 | Key Concepts

### 3.1 Reversible Reactions and Dynamic Equilibrium

For a general reaction:
$$aA + bB \rightleftharpoons cC + dD$$

At equilibrium, the concentrations of all species remain constant over time, not because reactions have stopped, but because **forward rate = reverse rate**. This is **dynamic** equilibrium.

### 3.2 The Equilibrium Constant ($K_c$)

$$K_c = \frac{[C]^c[D]^d}{[A]^a[B]^b}$$

Rules:
- Products in numerator, reactants in denominator, each raised to its stoichiometric coefficient.
- Pure solids and pure liquids are **omitted** (activity = 1).
- $K_c$ depends only on **temperature** (not on initial concentrations).
- $K_c \gg 1$: products favoured at equilibrium.
- $K_c \ll 1$: reactants favoured at equilibrium.
- $K_c$ has units (technically), but they are often omitted by convention in introductory texts.

### 3.3 $K_p$ for Gas-Phase Equilibria

For gas-phase reactions, partial pressures can be used:
$$K_p = \frac{P_C^c P_D^d}{P_A^a P_B^b}$$

**Conversion between $K_p$ and $K_c$:**
$$K_p = K_c(RT)^{\Delta n}$$
where $\Delta n = (\text{moles of gas products}) - (\text{moles of gas reactants})$.

### 3.4 Reaction Quotient ($Q$)

$Q$ has the same form as $K$ but with **current** (not equilibrium) concentrations. It tells us which way the reaction will shift:
- If $Q < K$: reaction shifts **right** (towards products) to reach equilibrium.
- If $Q > K$: reaction shifts **left** (towards reactants).
- If $Q = K$: system is at equilibrium.

### 3.5 ICE Tables

For a system starting with known concentrations, the ICE (Initial–Change–Equilibrium) method solves for equilibrium concentrations.

Example: $\ce{N2(g) + 3H2(g) <=> 2NH3(g)}$ with initial $[\ce{N2}]_0 = 1.0$ M, $[\ce{H2}]_0 = 3.0$ M, $[\ce{NH3}]_0 = 0$.

| | $\ce{N2}$ | $\ce{3H2}$ | $\ce{2NH3}$ |
|---|---|---|---|
| **I** | 1.0 | 3.0 | 0 |
| **C** | $-x$ | $-3x$ | $+2x$ |
| **E** | $1.0 - x$ | $3.0 - 3x$ | $2x$ |

$$K_c = \frac{(2x)^2}{(1.0 - x)(3.0 - 3x)^3}$$

Solve for $x$ (often requires approximation if $K$ is small or large).

**Approximation rule:** if $K$ is very small or initial concentration is relatively large, $x \ll [\text{initial}]$ and the change can be neglected. Always check that the approximation gives $x/[\text{initial}] < 5\%$.

### 3.6 Le Chatelier's Principle

*"If a system at equilibrium is disturbed, it will shift in the direction that opposes the disturbance."*

**Effects of changes:**

| Disturbance | Shift direction | Effect on $K$ |
|---|---|---|
| ↑ Concentration of reactant | Right | None |
| ↑ Concentration of product | Left | None |
| ↑ Volume (↓ pressure) | Side with more moles of gas | None |
| ↓ Volume (↑ pressure) | Side with fewer moles of gas | None |
| Add inert gas at constant V | No shift | None |
| Add inert gas at constant P | Shifts to side with more moles | None |
| ↑ Temperature (endothermic forward) | Right | $K$ increases |
| ↑ Temperature (exothermic forward) | Left | $K$ decreases |
| Add catalyst | No shift (rates equal) | None |

**Key insight:** Catalysts speed up **both** forward and reverse reactions equally, so $K$ is unchanged. Only temperature changes $K$.

### 3.7 Heterogeneous Equilibrium

Equilibria involving different phases. Solids and pure liquids are excluded from the equilibrium expression.

Examples:
$$\ce{CaCO3(s) <=> CaO(s) + CO2(g)}, \quad K_c = [\ce{CO2}]$$
$$\ce{CO2(g) + H2O(l) <=> H+(aq) + HCO3-(aq)}, \quad K_c = \frac{[\ce{H+}][\ce{HCO3-}]}{[\ce{CO2}]}$$

### 3.8 Equilibrium Position vs Equilibrium Constant

- **Equilibrium constant ($K$):** a fixed number at given $T$; tells us the ratio of products to reactants at equilibrium.
- **Equilibrium position:** the actual concentrations (or pressures) of each species at equilibrium; depends on initial conditions.

Different starting concentrations can give different equilibrium positions but the same $K$.

---

## 4 | Common Problem Types

### Type 1: Writing $K_c$ expression
> Write $K_c$ for $\ce{2SO2(g) + O2(g) <=> 2SO3(g)}$.

**Solution:**
$$K_c = \frac{[\ce{SO3}]^2}{[\ce{SO2}]^2[\ce{O2}]}$$

### Type 2: ICE calculation
> $\ce{2NO2(g) <=> N2O4(g)}$, $K_c = 4.5$ at 25 °C. Find equilibrium concentrations when $[\ce{NO2}]_0 = 0.10$ M.

**Solution:** Let $2x$ = amount of $\ce{N2O4}$ formed.
| | $\ce{2NO2}$ | $\ce{N2O4}$ |
|---|---|---|
| I | 0.10 | 0 |
| C | $-2x$ | $+x$ |
| E | $0.10 - 2x$ | $x$ |

$$K_c = \frac{x}{(0.10 - 2x)^2} = 4.5$$
Solving the quadratic: $x = 0.038$, so $[\ce{N2O4}] = 0.038$ M, $[\ce{NO2}] = 0.024$ M.

### Type 3: $K_p$ from $K_c$
> For $\ce{N2O4(g) <=> 2NO2(g)}$, $K_c = 4.5 \times 10^{-3}$ at 25 °C. Find $K_p$.

**Solution:** $\Delta n = 2 - 1 = 1$, $R = 0.0821$ L·atm/(mol·K), $T = 298$ K.
$$K_p = K_c(RT)^{\Delta n} = 4.5 \times 10^{-3} \times (0.0821 \times 298)^1 = 0.110$$

### Type 4: Direction of shift (Q vs K)
> $\ce{2H2(g) + CO(g) <=> CH3OH(g)}$, $K_c = 10.5$. Current concentrations: $[\ce{H2}] = 0.10$, $[\ce{CO}] = 0.020$, $[\ce{CH3OH}] = 1.5 \times 10^{-3}$. Which way does the reaction shift?

**Solution:**
$$Q = \frac{1.5 \times 10^{-3}}{(0.10)^2(0.020)} = \frac{1.5 \times 10^{-3}}{2.0 \times 10^{-4}} = 7.5$$
$Q < K$, so reaction shifts **right** (towards products).

### Type 5: Effect of pressure change
> For $\ce{2SO2(g) + O2(g) <=> 2SO3(g)}$, what happens when volume is halved?

**Solution:** Volume halves → all partial pressures double. 3 moles gas on left, 2 on right. By Le Chatelier, the system shifts to the side with fewer moles of gas → **right** (towards $\ce{SO3}$). $K$ is unchanged.

### Type 6: Effect of temperature on K
> For the exothermic reaction $\ce{N2(g) + 3H2(g) <=> 2NH3(g)}$, $\Delta H = -92$ kJ/mol. What happens to $K$ when $T$ increases?

**Solution:** Increasing $T$ shifts the exothermic direction backwards, so the reaction shifts **left** and $K$ **decreases**.

---

## 5 | Cross-Links

- [[05_Stoichiometry]] — mole ratios, balancing equations for $K$ expressions
- [[06_Solutions]] — concentration units in $K_c$
- [[07_Gases]] — partial pressure in $K_p$, $PV = nRT$
- [[08_Acids_and_Bases]] — $K_a$ and $K_b$ are equilibrium constants
- [[10_Ionic_Equilibrium]] — $K_{sp}$ (solubility product) is an equilibrium constant
- [[11_Thermochemistry]] — van 't Hoff equation: $K$ depends on $\Delta H$ and $T$
- [[12_Reaction_Kinetics]] — equilibrium when forward rate = reverse rate
