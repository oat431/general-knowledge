---
tags:
  - chemistry
  - advance
  - stoichiometry
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว311"]
---

# Stoichiometry — สมดุลเคมี

> *"Stoichiometry is the art of counting atoms and molecules — of relating the masses and amounts of substances in chemical reactions."* — Anonymous

Stoichiometry (สมดุลเคมี) is the study of the quantitative relationships between reactants (สารตั้งต้น) and products (ผลิตภัณฑ์) in a chemical reaction. It relies on an understanding of the mole, molar mass, balanced chemical equations, and mole ratios to predict the amounts of substances involved.

---

## 1 | Course Coverage

### ม.4 (ว311)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Mole concept (แนวคิดโมล), molar mass (มวลโมลาร์), balancing equations (ดุลสมการ), limiting reagent (สารกำหนดปริมาณ), % yield (ผลได้ร้อยละ), empirical/molecular formula (สูตรเอมพิริคัล/โมเลกุล), stoichiometric calculations | Balance equations, calculate mass/moles/volume, identify limiting reagent |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| โมล | Mole | $n$, หน่วยของปริมาณสาร |
| เลขอาโวกาโดร | Avogadro's number | $N_A = 6.022 \times 10^{23}$ |
| มวลโมลาร์ | Molar mass | $M$ (g/mol) |
| สารตั้งต้น | Reactant | สารที่เข้าทำปฏิกิริยา |
| ผลิตภัณฑ์ | Product | สารที่เกิดจากปฏิกิริยา |
| สารกำหนดปริมาณ | Limiting reagent | สารที่หมดก่อน |
| สารเกินพอ | Excess reagent | สารที่เหลือ |
| ผลได้ร้อยละ | Percent yield | $\%Y$ |
| สูตรเอมพิริคัล | Empirical formula | อัตราส่วนอะตอมอย่างง่าย |
| สูตรโมเลกุล | Molecular formula | จำนวนอะตอมจริง |

---

## 3 | Key Concepts

### 3.1 The Mole Concept

A mole (โมล) is the unit for the amount of substance: 1 mole = $6.022 \times 10^{23}$ particles (Avogadro's number).

**Relationships (ความสัมพันธ์):**

$$n = \frac{m}{M} = \frac{N}{N_A} = \frac{V}{22.4 \text{ (STP)}}$$

where:
- $n$ = number of moles (mol) (จำนวนโมล)
- $m$ = mass (g) (มวล)
- $M$ = molar mass (g/mol) (มวลโมลาร์)
- $N$ = number of particles (จำนวนอนุภาค)
- $V$ = volume (L, at STP) (ปริมาตร ที่ STP)

### 3.2 Molar Mass (มวลโมลาร์)

The mass of 1 mole of a substance, in g/mol, calculated as the sum of atomic masses in the formula.

**Example (ตัวอย่าง):**

$$M_{\ce{H2O}} = 2(1.008) + 16.00 = 18.02 \,\text{g/mol}$$

$$M_{\ce{Ca(OH)2}} = 40.08 + 2(16.00 + 1.008) = 74.10 \,\text{g/mol}$$

$$M_{\ce{Al2(SO4)3}} = 2(26.98) + 3(32.07 + 4 \times 16.00) = 342.17 \,\text{g/mol}$$

### 3.3 Balancing Chemical Equations

```mermaid
flowchart LR
    A["Balanced Equation"] --> B["Mole Ratios"]
    B --> C["Identify Limiting Reagent"]
    C --> D["Theoretical Yield"]
    D --> E["Compare to Actual Yield"]
    E --> F["Percent Yield"]
```

**Balancing rules (กฎการดุล):**
1. The number of atoms of each element must be equal on both sides (อะตอมแต่ละชนิดเท่ากันทั้ง 2 ข้าง)
2. Net charge must be equal (for ionic equations) (ประจุสุทธิเท่ากัน)
3. Balance H and O last (ดุล H และ O เป็นลำดับสุดท้าย)

**Example (ตัวอย่าง):** combustion of propane

$$\ce{C3H8 + 5O2 -> 3CO2 + 4H2O}$$

**Check (ตรวจสอบ):**
- C: 3 = 3 ✓
- H: 8 = 8 ✓
- O: 10 = 10 ✓

### 3.4 Mole Ratios & Stoichiometric Calculations

From a balanced equation, the coefficients in front of each species give the mole ratio (อัตราส่วนโมล).

**Example (ตัวอย่าง):** In $\ce{2H2 + O2 -> 2H2O}$ the mole ratio = $\ce{H2 : O2 : H2O} = 2 : 1 : 2$.

**Mass-to-Mass Conversion:**

$$\text{mass A} \xrightarrow{\div M_A} \text{mol A} \xrightarrow{\times \text{ratio}} \text{mol B} \xrightarrow{\times M_B} \text{mass B}$$

### 3.5 Limiting Reagent (สารกำหนดปริมาณ)

The reagent that is consumed completely first in a reaction, determining the maximum amount of product that can form (theoretical yield).

**How to find it (วิธีหา):**
1. Calculate the moles of product that each reactant could produce
2. The smallest value gives the theoretical yield, and the corresponding reactant is the limiting reagent

### 3.6 Percent Yield

$$\% \text{ Yield} = \frac{\text{actual yield}}{\text{theoretical yield}} \times 100$$

A value below 100% arises because: the reaction is incomplete, losses occur during transfer, and side reactions take place (ปฏิกิริยาไม่สมบูรณ์, สูญเสียระหว่างถ่ายเท, ปฏิกิริยาข้างเคียง).

### 3.7 Empirical & Molecular Formulas

**Empirical Formula (สูตรเอมพิริคัล):** The simplest whole-number ratio of atoms.

**Molecular Formula (สูตรโมเลกุล):** The actual number of atoms in a molecule.

$$\text{Molecular formula} = n \times \text{Empirical formula}$$

where

$$n = \frac{\text{Molar mass of compound}}{\text{Empirical formula mass}}$$

**Steps to find the EF from % composition (ขั้นตอนการหา EF จาก % composition):**
1. Convert % to grams (assume 100 g of sample) (เปลี่ยน % เป็นกรัม)
2. Divide by atomic mass → moles (หารด้วยมวลอะตอม → โมล)
3. Divide by the smallest value → ratio (หารด้วยค่าน้อยสุด → อัตราส่วน)
4. Round to whole numbers (multiply by a common factor if needed) (ปัดเศษเป็นจำนวนเต็ม ถ้าจำเป็นคูณด้วยตัวคูณร่วม)

### 3.8 Key Relationships (ความสัมพันธ์ที่สำคัญ)

| Relationship | Formula |
|---|---|
| Moles from mass (โมลจากมวล) | $n = m/M$ |
| Moles from number of particles (โมลจากจำนวนอนุภาค) | $n = N/N_A$ |
| Moles from gas volume (STP) (โมลจากปริมาตรแก๊ส STP) | $n = V/22.4$ |
| Moles from molarity (โมลจาก molarity) | $n = M \times V$ |
| Moles from partial pressure (โมลจาก partial pressure) | $n = PV/RT$ |
| Density of gas at STP (Density ของแก๊ส STP) | $d = M/22.4$ |

### 3.9 Reactions with Excess (ปฏิกิริยาที่มีสารเหลือ)

If a reaction uses A and B, and A is the limiting reagent:

- mol B used = (mol A) × (mole ratio B/A from the equation)
- mol B remaining = mol B initial − mol B used

### 3.10 Reactions in Solution

Use molarity:

$$M = \frac{n}{V} \quad \Rightarrow \quad n = M \times V$$

$$V_1 M_1 = V_2 M_2 \quad \text{(dilution)}$$

---

## 4 | Common Problem Types

### Type 1: Mole-to-Mass Conversion

> How many moles are in 14.1 g of sugar ($\ce{C12H22O11}$)?

**Solution:**

$$M = 12(12.01) + 22(1.008) + 11(16.00) = 342.3 \,\text{g/mol}$$

$$n = \frac{m}{M} = \frac{14.1}{342.3} = 0.0412 \,\text{mol}$$

### Type 2: Limiting Reagent

> Mix 4.00 mol of $\ce{N2}$ with 9.00 mol of $\ce{H2}$ in the reaction $\ce{N2 + 3H2 -> 2NH3}$. Which is the limiting reagent?

**Solution:**

- $\ce{N2}$ requires $\ce{H2}$ = $4.00 \times 3 = 12.00$ mol (only 9.00 mol available)
- $\ce{H2}$ requires $\ce{N2}$ = $9.00 / 3 = 3.00$ mol (4.00 mol available)
- **$\ce{H2}$ is the limiting reagent** (consumed first)
- $\ce{NH3}$ produced = $9.00 \times \frac{2}{3} = 6.00$ mol

### Type 3: Percent Yield

> In the reaction $\ce{CaCO3 -> CaO + CO2}$, 25.0 g of $\ce{CaCO3}$ produces 12.5 g of $\ce{CaO}$. Find the % yield.

**Solution:**

$$M_{\ce{CaCO3}} = 100.09, \quad M_{\ce{CaO}} = 56.08$$

$$\text{Theoretical: } 25.0 \times \frac{56.08}{100.09} = 14.0 \,\text{g CaO}$$

$$\% \text{ Yield} = \frac{12.5}{14.0} \times 100 = 89.3\%$$

### Type 4: Empirical Formula

> A compound contains C 40.0%, H 6.7%, O 53.3%. Find its empirical formula.

**Solution:**

(Assume 100 g → 40.0 g C, 6.7 g H, 53.3 g O)

- mol C = $40.0/12.01 = 3.33$
- mol H = $6.7/1.008 = 6.65$
- mol O = $53.3/16.00 = 3.33$

Divide by 3.33 → C:H:O = 1 : 2 : 1

**Empirical formula: $\ce{CH2O}$**

If the molar mass = 180 g/mol → $n = 180/30 = 6$ → Molecular formula = $\ce{C6H12O6}$ (glucose, กลูโคส)

### Type 5: Balancing Equations

> Balance the equation $\ce{Fe + O2 -> Fe2O3}$.

**Solution:**

$$\ce{4Fe + 3O2 -> 2Fe2O3}$$

- Fe: $4 = 2 \times 2 = 4$ ✓
- O: $3 \times 2 = 6 = 2 \times 3$ ✓

---

## 5 | Cross-Links

- [[01_Atomic_Structure]] — Atomic mass is the basis of molar mass
- [[06_Solutions]] — Molarity is used in solution stoichiometry
- [[07_Gases]] — Gas laws combine with stoichiometry
- [[../../Fundamental/10_Atoms_Elements_and_Compounds]] — Foundation of chemical equations
