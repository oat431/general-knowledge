---
tags:
  - chemistry
  - advance
  - ionic-equilibrium
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Ionic Equilibrium — สมดุลไอออน

> *"What dissolves and what precipitates are two sides of the same ionic ledger."* — Adapted from solubility chemistry

Ionic equilibrium extends the ideas of chemical equilibrium to solutions of sparingly soluble salts. It is the third equilibrium topic in ว312 and provides the conceptual bridge between the broad principles of $K$ (Topic 09) and the practical world of qualitative analysis, water treatment, and selective precipitation.

This note covers the solubility product $K_{sp}$, molar solubility, the common ion effect, conditions for precipitation (comparing $Q$ with $K_{sp}$), selective and fractional precipitation, the effect of pH on solubility, and the qualitative analysis of cations and anions.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | $K_{sp}$ and molar solubility, common ion effect, $Q$ vs $K_{sp}$, selective precipitation, pH and solubility, qualitative analysis (group reagents) | Write $K_{sp}$ expressions, calculate solubility, predict precipitation, plan separation schemes |
| **Semester 2** | (Not covered — see Thermochemistry, Kinetics, Electrochemistry) | — |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| สมดุลการละลาย | Solubility equilibrium | Solid ⇌ ions |
| ผลคูณไอออน | Ion product | $Q$ for ionic dissolution |
| ค่าคงที่ผลคูณไอออน | Solubility product | $K_{sp}$ |
| การละลายโมลาร์ | Molar solubility | mol/L of dissolved salt |
| สารละลายอิ่มตัว | Saturated solution | Equilibrium with solid |
| ไอออนร่วม | Common ion | Shared with dissolved salt |
| ผลของไอออนร่วม | Common ion effect | Lowers solubility |
| การตกตะกอน | Precipitation | $Q > K_{sp}$ |
| การตกตะกอนแบบเลือก | Selective precipitation | Separate by $K_{sp}$ |
| การตกตะกอนแบบเศษส่วน | Fractional precipitation | Gradual addition of reagent |
| สารตัวกลางตกตะกอน | Precipitating agent | Source of common ion |
| การวิเคราะห์คุณภาพ | Qualitative analysis | Identify ions in mixture |
| รีเอเจนต์กลุ่ม | Group reagent | Precipitates a class of ions |
| การละลายน้ำ | Aqueous solubility | Dissolves in water |
| ตะกอน | Precipitate | Insoluble solid |

---

## 3 | Key Concepts

### 3.1 Solubility Product ($K_{sp}$)

For a sparingly soluble salt dissolving in water:
$$\ce{CaF2(s) <=> Ca^2+(aq) + 2F-(aq)}$$
$$K_{sp} = [\ce{Ca^2+}][\ce{F-}]^2$$

General form: $\ce{A_mB_n(s) <=> mA^n+(aq) + nB^m-(aq)}$
$$K_{sp} = [\ce{A^{n+}}]^m \cdot [\ce{B^{m-}}]^n$$

**Important rules:**
- Solids are **omitted** from the expression.
- $K_{sp}$ depends only on temperature.
- Larger $K_{sp}$ = more soluble (in the same stoichiometric type).
- Compare $K_{sp}$ values only for salts of **same stoichiometry** (1:1 vs 1:2 give different scales).

### 3.2 Molar Solubility from $K_{sp}$

If $s$ is the molar solubility of $\ce{CaF2}$:
$[\ce{Ca^2+}] = s$, $[\ce{F-}] = 2s$.
$$K_{sp} = s \cdot (2s)^2 = 4s^3$$
$$s = \sqrt[3]{\frac{K_{sp}}{4}}$$

For $\ce{AgCl}$ (1:1): $K_{sp} = s^2$, so $s = \sqrt{K_{sp}}$.
For $\ce{Ag2CrO4}$ (2:1): $K_{sp} = (2s)^2 \cdot s = 4s^3$, so $s = \sqrt[3]{K_{sp}/4}$.
For $\ce{Ca3(PO4)2}$ (3:2): $K_{sp} = (3s)^3(2s)^2 = 108 s^5$.

### 3.3 Common Ion Effect

Adding a salt that shares an ion **decreases** the solubility of the original salt (Le Chatelier's principle).

Example: Solubility of $\ce{AgCl}$ in 0.10 M $\ce{NaCl}$:
$$K_{sp} = [\ce{Ag+}][\ce{Cl-}] = s(0.10 + s) \approx 0.10 s$$
$$s \approx \frac{K_{sp}}{0.10}$$

This $s$ is much smaller than $\sqrt{K_{sp}}$, the solubility in pure water.

### 3.4 Precipitation: $Q$ vs $K_{sp}$

The ion product $Q$ has the same form as $K_{sp}$ but with current concentrations:
- $Q < K_{sp}$: unsaturated, no precipitation, more solid can dissolve.
- $Q = K_{sp}$: saturated, at equilibrium.
- $Q > K_{sp}$: supersaturated, precipitation occurs until $Q = K_{sp}$.

### 3.5 Selective (Fractional) Precipitation

When a solution contains several cations that form insoluble salts with the same anion, the cation with the **smallest $K_{sp}$** (lowest required anion concentration) precipitates first.

To determine order: calculate the anion concentration needed to just begin precipitating each cation. The lowest threshold precipitates first.

**Example:** Solution 0.10 M in both $\ce{Cl-}$ and $\ce{CrO4^2-}$. Adding $\ce{Ag+}$ gradually. With $K_{sp}(\ce{AgCl}) = 1.8 \times 10^{-10}$ and $K_{sp}(\ce{Ag2CrO4}) = 1.1 \times 10^{-12}$:
- To start $\ce{AgCl}$ ppt: $[\ce{Ag+}] > K_{sp}/[\ce{Cl-}] = 1.8 \times 10^{-9}$ M.
- To start $\ce{Ag2CrO4}$ ppt: $[\ce{Ag+}] > \sqrt{K_{sp}/[\ce{CrO4^2-}]} = \sqrt{1.1 \times 10^{-11}} = 3.3 \times 10^{-6}$ M.
- $\ce{Ag2CrO4}$ precipitates first, then $\ce{AgCl}$ when $[\ce{Ag+}]$ exceeds $1.8 \times 10^{-9}$ M.

### 3.6 Effect of pH on Solubility

For salts containing **basic anions** (conjugate bases of weak acids), solubility **increases** as pH decreases. The anion reacts with $\ce{H+}$:

$$\ce{CaCO3(s) <=> Ca^2+(aq) + CO3^2-(aq)}$$
$$\ce{CO3^2- + H+ <=> HCO3-}$$
$$\ce{HCO3- + H+ <=> H2CO3 -> H2O + CO2(g)}$$

Adding acid shifts both equilibria right, dissolving more $\ce{CaCO3}$. This is why limestone caves form in acidic groundwater, and why antacid tablets work in the stomach.

For salts of strong acids (e.g. $\ce{AgCl}$, $\ce{BaSO4}$), pH has little effect on solubility.

### 3.7 Qualitative Analysis of Cations

The IPST curriculum uses a classical scheme to identify common cations by selective precipitation with group reagents.

| Group | Cations | Group reagent | Precipitate |
|---|---|---|---|
| 1 | $\ce{Ag+}$, $\ce{Pb^2+}$, $\ce{Hg2^2+}$ | Dilute $\ce{HCl}$ | Chlorides ($\ce{AgCl}$, $\ce{PbCl2}$, $\ce{Hg2Cl2}$) |
| 2 | $\ce{Cu^2+}$, $\ce{Cd^2+}$, $\ce{Bi^3+}$, $\ce{Hg^2+}$, $\ce{Pb^2+}$ (residual), $\ce{As^3+}$, $\ce{Sb^3+}$, $\ce{Sn^4+}$ | $\ce{H2S}$ in acidic solution | Sulfides |
| 3 | $\ce{Fe^3+}$, $\ce{Al^3+}$, $\ce{Cr^3+}$ | $\ce{NH3}$ + $\ce{NH4Cl}$ | Hydroxides |
| 4 | $\ce{Zn^2+}$, $\ce{Mn^2+}$, $\ce{Ni^2+}$, $\ce{Co^2+}$ | $\ce{H2S}$ in basic solution | Sulfides |
| 5 | $\ce{Ba^2+}$, $\ce{Sr^2+}$, $\ce{Ca^2+}$ | $\ce{(NH4)2CO3}$ | Carbonates |
| 6 | $\ce{Na+}$, $\ce{K+}$, $\ce{NH4+}$ | (no group reagent; identified by flame test or Nessler's reagent) | Soluble |

This separation exploits (a) different $K_{sp}$ values of similar salts, and (b) pH control.

---

## 4 | Common Problem Types

### Type 1: $K_{sp}$ from solubility
> The solubility of $\ce{PbI2}$ is $1.5 \times 10^{-3}$ mol/L. Find $K_{sp}$.

**Solution:** $\ce{PbI2(s) <=> Pb^2+(aq) + 2I-(aq)}$
$[\ce{Pb^2+}] = s = 1.5 \times 10^{-3}$, $[\ce{I-}] = 2s = 3.0 \times 10^{-3}$
$$K_{sp} = (1.5 \times 10^{-3})(3.0 \times 10^{-3})^2 = 1.35 \times 10^{-8}$$

### Type 2: Solubility from $K_{sp}$
> $K_{sp}(\ce{Ag2CrO4}) = 1.1 \times 10^{-12}$. Find molar solubility.

**Solution:** $K_{sp} = 4s^3$
$$s = \sqrt[3]{\frac{1.1 \times 10^{-12}}{4}} = 6.5 \times 10^{-5}\ \text{M}$$

### Type 3: Will precipitation occur?
> 100 mL of 0.010 M $\ce{NaCl}$ is mixed with 100 mL of 0.020 M $\ce{AgNO3}$. Will $\ce{AgCl}$ precipitate? $K_{sp}(\ce{AgCl}) = 1.8 \times 10^{-10}$.

**Solution:** After mixing (volume doubles): $[\ce{Cl-}] = 0.0050$ M, $[\ce{Ag+}] = 0.010$ M.
$$Q = [\ce{Ag+}][\ce{Cl-}] = (0.010)(0.0050) = 5.0 \times 10^{-5}$$
$Q \gg K_{sp}$, so **precipitation occurs**.

### Type 4: Common ion effect
> Find solubility of $\ce{AgCl}$ in 0.20 M $\ce{NaCl}$. $K_{sp} = 1.8 \times 10^{-10}$.

**Solution:** $[\ce{Cl-}] \approx 0.20$ M (large excess). Let $s = [\ce{Ag+}]$.
$$K_{sp} = s \cdot 0.20 = 1.8 \times 10^{-10}$$
$$s = 9.0 \times 10^{-10}\ \text{M}$$
(Compare to $\sqrt{K_{sp}} = 1.34 \times 10^{-5}$ M in pure water — about 15 000× less soluble.)

### Type 5: Selective precipitation
> A solution is 0.10 M in $\ce{Pb^2+}$ and 0.10 M in $\ce{Sr^2+}$. $\ce{Na2SO4}$ is added gradually. Which precipitates first? $K_{sp}(\ce{PbSO4}) = 1.6 \times 10^{-8}$, $K_{sp}(\ce{SrSO4}) = 3.2 \times 10^{-7}$.

**Solution:** Required $[\ce{SO4^2-}]$:
- For $\ce{PbSO4}$: $[\ce{SO4^2-}] > K_{sp}/[\ce{Pb^2+}] = 1.6 \times 10^{-7}$ M
- For $\ce{SrSO4}$: $[\ce{SO4^2-}] > K_{sp}/[\ce{Sr^2+}] = 3.2 \times 10^{-6}$ M

$\ce{PbSO4}$ precipitates first (lower threshold).

---

## 5 | Cross-Links

- [[08_Acids_and_Bases]] — pH effects on basic anions; $K_a$/$K_b$ of conjugate acid-base pairs
- [[09_Chemical_Equilibrium]] — $K_{sp}$ is a special case of $K_c$; $Q$ vs $K$ rule
- [[05_Stoichiometry]] — mole calculations for precipitation yields
- [[06_Solutions]] — concentration units, dilution
- [[13_Electrochemistry]] — solubility and electrode potential (Nernst)
- [[../Biology/02_Genetics_Evolution_and_Ecology|Biology]] — kidney stones, biomineralization
