---
tags:
  - chemistry
  - advance
  - gases
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว311"]
---

# Gases — แก๊ส

> *"Gases are the most disordered state of matter, yet they obey some of the simplest and most elegant laws in nature."* — Anonymous

Gases (แก๊ส) are a state of matter in which the particles are far apart, move freely, and possess high kinetic energy. They are studied through the kinetic molecular theory and a set of simple laws — Boyle's, Charles's, Avogadro's, Dalton's, and Graham's — that describe the relationships between pressure (P), volume (V), temperature (T), and amount (n).

---

## 1 | Course Coverage

### ม.4 (ว311)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Kinetic Molecular Theory, Boyle/Charles/Avogadro's Law, Ideal Gas Law ($PV=nRT$), Dalton's Law, Graham's Law, Real gas deviations | Apply gas laws to calculate P, V, T, n; explain gas behavior |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ความดัน | Pressure | $P$ (atm, Pa, mmHg, torr) |
| ปริมาตร | Volume | $V$ (L, m³) |
| อุณหภูมิ | Temperature | $T$ (K เท่านั้น) |
| จำนวนโมล | Moles | $n$ (mol) |
| ค่าคงที่แก๊ส | Gas constant | $R = 0.0821$ L·atm/(mol·K) |
| ความดันย่อย | Partial pressure | $P_i$ |
| กฎของบอยล์ | Boyle's law | $P \propto 1/V$ ที่ T, n คงที่ |
| กฎของชาร์ลส์ | Charles's law | $V \propto T$ ที่ P, n คงที่ |
| กฎของอาโวกาโดร | Avogadro's law | $V \propto n$ ที่ P, T คงที่ |
| กฎของดาลตัน | Dalton's law | $P_{total} = \sum P_i$ |
| กฎของเกรแฮม | Graham's law | อัตรา diffusion $\propto 1/\sqrt{M}$ |

---

## 3 | Key Concepts

### 3.1 Kinetic Molecular Theory (KMT)

**Postulates (สมมติฐาน):**

1. A gas consists of a large number of small particles whose separation is much greater than their size (แก๊สประกอบด้วยอนุภาคเล็ก ๆ จำนวนมาก ระยะห่างระหว่างอนุภาคมากกว่าขนาดอนุภาค)
2. The particles are in continuous, random motion (อนุภาคเคลื่อนที่อย่างต่อเนื่องและสุ่ม)
3. No forces of attraction or repulsion act between particles (except during collisions) (ไม่มีแรงดึงดูด/ผลักระหว่างอนุภาค ยกเว้นการชน)
4. Collisions between particles or with the walls are perfectly elastic (การชนเป็นแบบยืดหยุ่นสมบูรณ์)
5. The average kinetic energy is proportional to the absolute temperature (Kelvin) (พลังงานจลน์เฉลี่ย $\propto T$)

**Explanation (อธิบาย):**
- Pressure: arises from collisions of particles with the walls
- Temperature: proportional to the average kinetic energy
- Diffusion: the spreading of a gas through space

### 3.2 Units & Conversions

**Pressure (ความดัน):**

$$1 \,\text{atm} = 101.325 \,\text{kPa} = 760 \,\text{mmHg} = 760 \,\text{torr} = 1.01325 \times 10^5 \,\text{Pa}$$

**Temperature (อุณหภูมิ):** Always use **Kelvin (K เสมอ)**

$$T(K) = T(°C) + 273.15$$

**Volume (ปริมาตร):** 1 L = 1 dm³ = $10^{-3}$ m³

**Value of R (ค่า R):**

| $R$ value | Units |
|---|---|
| 0.0821 | L·atm/(mol·K) |
| 8.314 | J/(mol·K) |
| 62.36 | L·torr/(mol·K) |

### 3.3 Boyle's Law (Pressure–Volume) (กฎของบอยล์)

At constant temperature and number of moles:

$$P_1V_1 = P_2V_2 \quad \text{or} \quad P \propto \frac{1}{V}$$

**Characteristic (ลักษณะ):** Increasing P decreases V (inverse relationship).

### 3.4 Charles's Law (Volume–Temperature) (กฎของชาร์ลส์)

At constant pressure and number of moles:

$$\frac{V_1}{T_1} = \frac{V_2}{T_2} \quad \text{or} \quad V \propto T$$

**Characteristic (ลักษณะ):** Increasing T increases V (directly proportional).

At $T = 0$ K → $V = 0$ (absolute zero).

### 3.5 Gay-Lussac's Law (Pressure–Temperature)

At constant volume and number of moles:

$$\frac{P_1}{T_1} = \frac{P_2}{T_2} \quad \text{or} \quad P \propto T$$

### 3.6 Avogadro's Law (Volume–Moles) (กฎของอาโวกาโดร)

At constant pressure and temperature:

$$\frac{V_1}{n_1} = \frac{V_2}{n_2} \quad \text{or} \quad V \propto n$$

**Important consequence (ผลสำคัญ):** At STP (0°C, 1 atm) 1 mole of gas occupies 22.4 L.

At RTP (25°C, 1 atm) → **24.0 L/mol**

### 3.7 Combined Gas Law

Combines Boyle, Charles, and Gay-Lussac:

$$\frac{P_1V_1}{T_1} = \frac{P_2V_2}{T_2}$$

### 3.8 Ideal Gas Law

Combines all four variables P, V, T, n:

$$\boxed{PV = nRT}$$

or equivalently

$$PV = \frac{m}{M}RT$$

The molar mass of a gas can therefore be obtained from:

$$M = \frac{mRT}{PV}$$

### 3.9 Dalton's Law of Partial Pressures

In a mixture of gases, the total pressure equals the sum of the partial pressures (ในแก๊สผสม ความดันรวม = ผลรวมความดันย่อย):

$$P_{total} = P_1 + P_2 + P_3 + ... = \sum P_i$$

**Mole fraction:**

$$x_i = \frac{n_i}{n_{total}}$$

$$P_i = x_i \cdot P_{total}$$

**Example (ตัวอย่าง):** Air is $\ce{N2}$ 78%, $\ce{O2}$ 21%, others 1%.
- $P_{\ce{N2}} = 0.78 \times P_{atm}$

### 3.10 Graham's Law of Effusion (กฎของเกรแฮม)

**Effusion:** A gas escapes through a tiny hole into a vacuum (แก๊สไหลผ่านรูเล็ก ๆ ลงสู่สุญญากาศ).

$$\frac{r_1}{r_2} = \sqrt{\frac{M_2}{M_1}}$$

where $r$ = rate of effusion, $M$ = molar mass.

**A heavier gas (larger M) effuses more slowly (แก๊สที่หนักกว่าจะ effuse ช้ากว่า).**

### 3.11 Gas Stoichiometry

**At STP:** 1 mol of gas = 22.4 L

**Formulas (สูตร):**

$$n = \frac{V}{22.4} \quad \text{(STP)}$$

**General:**

$$n = \frac{PV}{RT}$$

**Example (ตัวอย่าง):**

$$\ce{2H2(g) + O2(g) -> 2H2O(g)}$$

Using 5.0 L of $\ce{H2}$ → $\ce{O2}$ required = $5.0 / 2 = 2.5$ L, gives $\ce{H2O}$ = 5.0 L

### 3.12 Collecting Gas Over Water (การเก็บแก๊สเหนือน้ำ)

When a gas is collected by water displacement:

$$P_{gas} = P_{atm} - P_{water\ vapor}$$

($P_{water\ vapor}$ depends on temperature; look it up in a table.)

### 3.13 Real Gases — Deviations from Ideal Behavior

**Real gases (แก๊สจริง)** deviate from ideal behavior when:
- Pressure is high (ความดันสูง)
- Temperature is low (อุณหภูมิต่ำ)
- Molecules are polar or large (โมเลกุลมีขั้ว/ขนาดใหญ่)

**van der Waals equation (สมการ van der Waals):**

$$\left(P + \frac{an^2}{V^2}\right)(V - nb) = nRT$$

where:
- $a$ = correction for intermolecular attraction
- $b$ = correction for finite molecular volume
- $\frac{an^2}{V^2}$ = attractive force term
- $nb$ = excluded volume

**Compressibility factor (Z):**

$$Z = \frac{PV}{nRT}$$

- $Z = 1$: ideal
- $Z < 1$: attractive forces dominate
- $Z > 1$: repulsive forces dominate

### 3.14 Summary of Gas Laws (สรุปกฎแก๊ส)

| Law | Variables | Constant | Formula |
|---|---|---|---|
| Boyle | P, V | T, n | $P_1V_1 = P_2V_2$ |
| Charles | V, T | P, n | $V_1/T_1 = V_2/T_2$ |
| Gay-Lussac | P, T | V, n | $P_1/T_1 = P_2/T_2$ |
| Avogadro | V, n | P, T | $V_1/n_1 = V_2/n_2$ |
| Combined | P, V, T | n | $P_1V_1/T_1 = P_2V_2/T_2$ |
| Ideal | P, V, T, n | - | $PV = nRT$ |
| Dalton | $P_i$ | V, T | $P_{tot} = \sum P_i$ |
| Graham | Effusion rate, M | - | $r \propto 1/\sqrt{M}$ |

---

## 4 | Common Problem Types

### Type 1: Ideal Gas Law

> 8.0 g of $\ce{O2}$ is in a 5.0 L container at 27°C. Find the pressure.

**Solution:**

$M_{\ce{O2}} = 32.00 \,\text{g/mol}, \quad n = 8.0/32.00 = 0.25 \,\text{mol}$

$T = 27 + 273 = 300 \,\text{K}$

$$P = \frac{nRT}{V} = \frac{0.25 \times 0.0821 \times 300}{5.0} = 1.23 \,\text{atm}$$

### Type 2: Combined Gas Law

> A gas at 1.5 atm, 25°C, 2.0 L is compressed to 0.50 L at 50°C. Find the new pressure.

**Solution:**

$$\frac{P_1V_1}{T_1} = \frac{P_2V_2}{T_2}$$

$$\frac{1.5 \times 2.0}{298} = \frac{P_2 \times 0.50}{323}$$

$$P_2 = \frac{1.5 \times 2.0 \times 323}{298 \times 0.50} = 6.5 \,\text{atm}$$

### Type 3: Dalton's Law

> A gas mixture contains 2.0 mol $\ce{N2}$, 1.0 mol $\ce{O2}$, and 0.5 mol $\ce{He}$ in a 10 L container at 300 K. Find $P_{total}$.

**Solution:**

$n_{total} = 3.5 \,\text{mol}$

$$P_{total} = \frac{nRT}{V} = \frac{3.5 \times 0.0821 \times 300}{10} = 8.62 \,\text{atm}$$

Or compute the partial pressure of each gas and add them (หรือคำนวณ partial pressure แต่ละตัวแล้วรวม).

### Type 4: Graham's Law

> $\ce{H2}$ effuses in 30 s. An unknown gas effuses in 120 s. Identify the gas ($M_{\ce{H2}} = 2$).

**Solution:**

$$\frac{r_1}{r_2} = \sqrt{\frac{M_2}{M_1}}$$

Rate = $1/t$, so $\frac{t_2}{t_1} = \sqrt{\frac{M_2}{M_1}}$

$$\frac{120}{30} = \sqrt{\frac{M_2}{2}}$$

$$16 = \frac{M_2}{2} \Rightarrow M_2 = 32 \quad \text{(e.g. \ce{O2})}$$

### Type 5: Gas Stoichiometry

> Burn 16 g of $\ce{CH4}$ with excess $\ce{O2}$. How many liters of $\ce{CO2}$ are produced at STP?

**Solution:**

$\ce{CH4 + 2O2 -> CO2 + 2H2O}$

$n_{\ce{CH4}} = 16/16 = 1.0 \,\text{mol}$

$\ce{CO2}$ produced = $1.0 \,\text{mol}$

$V = 1.0 \times 22.4 = 22.4 \,\text{L}$

### Type 6: Molar Mass from Gas Density

> A gas has density 2.5 g/L at STP. Find its molar mass.

**Solution:**

$$M = d \times 22.4 = 2.5 \times 22.4 = 56 \,\text{g/mol}$$

### Type 7: Collecting Gas Over Water

> $\ce{H2}$ is collected over water at 25°C, $P_{atm}$ = 755 mmHg, $P_{\ce{H2O}}$ = 24 mmHg; 250 mL of gas is collected. How many moles?

**Solution:**

$P_{\ce{H2}} = 755 - 24 = 731 \,\text{mmHg} = 731/760 = 0.962 \,\text{atm}$

$T = 298 \,\text{K}, \quad V = 0.250 \,\text{L}$

$$n = \frac{PV}{RT} = \frac{0.962 \times 0.250}{0.0821 \times 298} = 9.83 \times 10^{-3} \,\text{mol}$$

---

## 5 | Cross-Links

- [[05_Stoichiometry]] — Mole ratios are used in gas stoichiometry
- [[06_Solutions]] — Henry's Law (gases in solution)
- [[04_Intermolecular_Forces]] — IMFs affect the deviation of real gases from ideal
- [[../../Advance/physics/02_Kinematics|Physics Kinematics]] — KMT uses kinematics
- [[../../Advance/physics/05_Thermodynamics|Physics Thermodynamics]] — Temperature and kinetic energy
