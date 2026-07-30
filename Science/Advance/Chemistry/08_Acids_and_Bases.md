---
tags:
  - chemistry
  - advance
  - acids-bases
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Acids and Bases — กรดและเบส

> *"Acids and bases are the yin and yang of chemistry — every proton donated must be accepted."* — Adapted from Brønsted-Lowry

Acids (กรด) and bases (เบส) are among the most important classes of compounds in chemistry. They govern everything from the taste of food to the functioning of biological enzymes and the pH of our blood. The study of acids and bases opens Semester 1 of the ว312 curriculum and lays the groundwork for ionic equilibrium, buffers, and electrochemistry.

This note covers the three theories of acids and bases (Arrhenius, Brønsted-Lowry, Lewis), conjugate acid-base pairs, the pH and pOH scales, strong versus weak electrolytes, the acid dissociation constant $K_a$ and base dissociation constant $K_b$, hydrolysis of salts, buffer solutions, the Henderson-Hasselbalch equation, and acid-base titration curves.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Arrhenius/Brønsted-Lowry/Lewis theories, conjugate pairs, pH/pOH, strong vs weak acids & bases, $K_a$/$K_b$, hydrolysis, buffers, Henderson-Hasselbalch, titration curves | Calculate pH of strong/weak acids & bases, build ICE tables, choose indicators, interpret titration curves |
| **Semester 2** | (Not covered — see Thermochemistry, Kinetics, Electrochemistry) | — |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| กรด | Acid | Proton (H⁺) donor |
| เบส | Base | Proton (H⁺) acceptor |
| กรดแก่ | Strong acid | Fully dissociates (e.g. $\ce{HCl}$, $\ce{HNO3}$) |
| กรดอ่อน | Weak acid | Partially dissociates (e.g. $\ce{CH3COOH}$) |
| เบสแก่ | Strong base | Fully dissociates (e.g. $\ce{NaOH}$, $\ce{KOH}$) |
| เบสอ่อน | Weak base | Partially dissociates (e.g. $\ce{NH3}$) |
| คู่กรด-เบส | Conjugate acid-base pair | Differ by one $\ce{H+}$ |
| แอมโฟเทอริก | Amphoteric | Can act as acid or base |
| ไฮโดรเนียม | Hydronium ion | $\ce{H3O+}$ |
| ไฮดรอกไซด์ | Hydroxide | $\ce{OH-}$ |
| ค่า pH | pH (potential of hydrogen) | $-\log[\ce{H+}]$ |
| ค่า pOH | pOH | $-\log[\ce{OH-}]$ |
| ค่าคงที่การแตกตัว | Dissociation constant | $K_a$ (acid), $K_b$ (base) |
| สารละลายบัฟเฟอร์ | Buffer solution | Resists pH change |
| การไทเทรต | Titration | Volumetric analysis |
| อินดิเคเตอร์ | Indicator | Colour change at endpoint |
| จุดสมมูล | Equivalence point | Moles acid = moles base |
| จุดยุติ | Endpoint | Indicator colour change |
| ไฮโดรไลซิส | Hydrolysis | Salt reacts with water |

---

## 3 | Key Concepts

### 3.1 Three Theories of Acids and Bases

**Arrhenius Theory (1884):**
- Acid: substance that produces $\ce{H+}$ in water (e.g. $\ce{HCl -> H+ + Cl-}$)
- Base: substance that produces $\ce{OH-}$ in water (e.g. $\ce{NaOH -> Na+ + OH-}$)
- Limitation: restricted to aqueous solutions; doesn't explain $\ce{NH3}$ as base.

**Brønsted-Lowry Theory (1923):**
- Acid: proton ($\ce{H+}$) donor
- Base: proton acceptor
- Reaction is a proton transfer: $\ce{HA + B <=> A- + HB+}$
- Every acid–base reaction has **two conjugate pairs**.
- Example: $\ce{NH3 + H2O <=> NH4+ + OH-}$ — $\ce{H2O}$ is acid, $\ce{NH3}$ is base; $\ce{NH4+}$ and $\ce{NH3}$ form one conjugate pair, $\ce{H2O}$ and $\ce{OH-}$ form the other.

**Lewis Theory (1923):**
- Acid: electron-pair acceptor (electrophile)
- Base: electron-pair donor (nucleophile)
- Most general — covers all Brønsted-Lowry reactions plus those without $\ce{H+}$ (e.g. $\ce{BF3 + NH3 -> F3B-NH3}$).
- Used heavily in organic chemistry and coordination chemistry.

### 3.2 Conjugate Acid-Base Pairs

In $\ce{HA <=> H+ + A-}$:
- $\ce{HA}$ is the acid; $\ce{A-}$ is its **conjugate base**.
- The stronger the acid, the weaker its conjugate base.
- Water is amphoteric: $\ce{H2O <=> H+ + OH-}$ and $\ce{H2O + H+ -> H3O+}$.

### 3.3 Water Autoionization

Pure water self-ionizes:
$$\ce{2H2O <=> H3O+ + OH-}$$

At 25 °C: $K_w = [\ce{H3O+}][\ce{OH-}] = 1.0 \times 10^{-14}$

Neutral water: $[\ce{H+}] = [\ce{OH-}] = 1.0 \times 10^{-7}$ M

### 3.4 pH and pOH Scales

$$\text{pH} = -\log[\ce{H+}] \qquad \text{pOH} = -\log[\ce{OH-}]$$

At 25 °C: $\text{pH} + \text{pOH} = 14$

| Solution | $[\ce{H+}]$ | pH |
|---|---|---|
| Acidic | $> 10^{-7}$ | $< 7$ |
| Neutral | $= 10^{-7}$ | $= 7$ |
| Basic | $< 10^{-7}$ | $> 7$ |

### 3.5 Strong vs Weak Acids and Bases

**Strong acids** (7 in IPST curriculum): $\ce{HCl}$, $\ce{HBr}$, $\ce{HI}$, $\ce{HNO3}$, $\ce{H2SO4}$ (first proton), $\ce{HClO4}$, $\ce{HClO3}$.
**Strong bases**: Group 1 hydroxides ($\ce{LiOH}$, $\ce{NaOH}$, $\ce{KOH}$, ...) and heavy Group 2 hydroxides ($\ce{Ca(OH)2}$, $\ce{Sr(OH)2}$, $\ce{Ba(OH)2}$).

For strong acids/bases: complete dissociation, so $[\ce{H+}]$ (or $[\ce{OH-}]$) = initial concentration.

**Weak acids/bases**: partial dissociation, characterized by $K_a$ or $K_b$.

For weak acid $\ce{HA <=> H+ + A-}$:
$$K_a = \frac{[\ce{H+}][\ce{A-}]}{[\ce{HA}]}$$

For weak base $\ce{B + H2O <=> BH+ + OH-}$:
$$K_b = \frac{[\ce{BH+}][\ce{OH-}]}{[\ce{B}]}$$

**Relationship for conjugate pairs**: $K_a \cdot K_b = K_w = 1.0 \times 10^{-14}$ at 25 °C.
Larger $K_a$ → stronger acid → weaker conjugate base.

### 3.6 Hydrolysis of Salts

Salts of strong acid + strong base (e.g. $\ce{NaCl}$) → neutral (pH = 7).
Salts of strong acid + weak base (e.g. $\ce{NH4Cl}$) → acidic ($\ce{NH4+}$ hydrolyzes).
Salts of weak acid + strong base (e.g. $\ce{CH3COONa}$) → basic ($\ce{CH3COO-}$ hydrolyzes).
Salts of weak acid + weak base (e.g. $\ce{CH3COONH4}$) → depends on $K_a$ vs $K_b$.

### 3.7 Buffer Solutions

A **buffer** resists pH change upon addition of small amounts of strong acid or base. Two types:
- **Acidic buffer**: weak acid + its conjugate base (e.g. $\ce{CH3COOH / CH3COONa}$)
- **Basic buffer**: weak base + its conjugate acid (e.g. $\ce{NH3 / NH4Cl}$)

**Henderson-Hasselbalch equation:**
$$\text{pH} = \text{p}K_a + \log\frac{[\text{A}^-]}{[\text{HA}]}$$

When $[\text{A}^-] = [\text{HA}]$, $\text{pH} = \text{p}K_a$ — the buffer's most effective pH.
Effective buffer range: $\text{pH} = \text{p}K_a \pm 1$.

### 3.8 Acid-Base Titration Curves

**Strong acid–strong base**: pH rises sharply at equivalence; pH = 7 at equivalence.
**Weak acid–strong base**: pH > 7 at equivalence (conjugate base hydrolyzes); buffer region visible at $\text{pH} = \text{p}K_a$ (half-equivalence point).
**Weak base–strong acid**: pH < 7 at equivalence.

**Indicators** (selected):
| Indicator | pH range | Colour change |
|---|---|---|
| Methyl orange | 3.1 – 4.4 | red → yellow |
| Bromothymol blue | 6.0 – 7.6 | yellow → blue |
| Phenolphthalein | 8.2 – 10.0 | colourless → pink |
| Litmus | 4.5 – 8.3 | red → blue |

Choose indicator whose range brackets the equivalence pH.

---

## 4 | Common Problem Types

### Type 1: pH of strong acid
> Find pH of $0.025$ M $\ce{HCl}$.

**Solution:** Strong acid, fully dissociates: $[\ce{H+}] = 0.025$
$$\text{pH} = -\log(0.025) = 1.60$$

### Type 2: pH of weak acid (ICE table)
> Find pH of $0.10$ M acetic acid ($\ce{CH3COOH}$), $K_a = 1.8 \times 10^{-5}$.

**Solution:** ICE table: $\ce{CH3COOH <=> H+ + CH3COO-}$
$$K_a = \frac{x^2}{0.10 - x} \approx \frac{x^2}{0.10} = 1.8 \times 10^{-5}$$
$$x = [\ce{H+}] = \sqrt{1.8 \times 10^{-6}} = 1.34 \times 10^{-3}\ \text{M}$$
$$\text{pH} = -\log(1.34 \times 10^{-3}) = 2.87$$

### Type 3: Buffer pH (Henderson-Hasselbalch)
> A buffer contains $0.50$ M $\ce{CH3COOH}$ and $0.30$ M $\ce{CH3COONa}$. $K_a = 1.8 \times 10^{-5}$. Find pH.

**Solution:**
$$\text{pH} = \text{p}K_a + \log\frac{[\text{A}^-]}{[\text{HA}]} = -\log(1.8 \times 10^{-5}) + \log\frac{0.30}{0.50}$$
$$\text{pH} = 4.74 + \log(0.60) = 4.74 - 0.22 = 4.52$$

### Type 4: $K_b$ from $K_a$
> For $\ce{NH3}$ (conjugate acid $\ce{NH4+}$), $K_a(\ce{NH4+}) = 5.6 \times 10^{-10}$. Find $K_b(\ce{NH3})$.

**Solution:** $K_a \cdot K_b = K_w = 1.0 \times 10^{-14}$
$$K_b = \frac{10^{-14}}{5.6 \times 10^{-10}} = 1.79 \times 10^{-5}$$

### Type 5: pH of salt solution (hydrolysis)
> Find pH of $0.10$ M $\ce{CH3COONa}$. $K_a(\ce{CH3COOH}) = 1.8 \times 10^{-5}$.

**Solution:** $\ce{CH3COO- + H2O <=> CH3COOH + OH-}$
$$K_b = \frac{K_w}{K_a} = \frac{10^{-14}}{1.8 \times 10^{-5}} = 5.56 \times 10^{-10}$$
$$[\ce{OH-}] = \sqrt{K_b \cdot C} = \sqrt{5.56 \times 10^{-10} \times 0.10} = 7.45 \times 10^{-6}\ \text{M}$$
$$\text{pOH} = 5.13, \quad \text{pH} = 8.87$$

### Type 6: Titration stoichiometry
> $25.0$ mL of $0.100$ M $\ce{NaOH}$ is titrated with $0.050$ M $\ce{HCl}$. Find volume of $\ce{HCl}$ at equivalence.

**Solution:** Moles $\ce{NaOH}$ = $0.025 \times 0.100 = 2.5 \times 10^{-3}$ mol.
At equivalence: moles $\ce{HCl}$ = moles $\ce{NaOH}$.
$$V = \frac{2.5 \times 10^{-3}}{0.050} = 0.050\ \text{L} = 50.0\ \text{mL}$$

---

## 5 | Cross-Links

- [[../../Fundamental/12_Acids_Bases_and_Salts]] — foundation from ม.1–3
- [[05_Stoichiometry]] — stoichiometry prerequisite for titration calculations
- [[06_Solutions]] — concentration units (M, dilution)
- [[07_Gases]] — partial pressure analogue of concentration in $K_c$/$K_p$
- [[09_Chemical_Equilibrium]] — $K_a$ and $K_b$ are equilibrium constants
- [[10_Ionic_Equilibrium]] — buffers connect to salt hydrolysis and $K_{sp}$
- [[13_Electrochemistry]] — pH electrodes, Nernst equation
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — logarithms, exponentials
