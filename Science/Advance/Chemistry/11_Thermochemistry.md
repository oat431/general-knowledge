---
tags:
  - chemistry
  - advance
  - thermochemistry
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Thermochemistry — อุณหเคมี

> *"Energy is conserved; it is merely transformed, transported, and stored — and the heat released or absorbed by a reaction is the most honest measure of its progress."* — Adapted from the First Law

Thermochemistry is the branch of chemistry that studies the heat absorbed or released during chemical reactions. It is the first topic of Semester 2 in ว312, bridging the equilibrium-flavoured first semester (Topics 08–10) with the rate-flavoured and electron-flavoured topics that follow. Beyond the classroom, thermochemistry underlies combustion engines, metabolism, calorimetry in food science, and the design of industrial reactors.

This note covers enthalpy ($\Delta H$), endothermic and exothermic processes, calorimetry, Hess's law, standard enthalpies of formation, bond energies, entropy ($\Delta S$), Gibbs free energy ($\Delta G = \Delta H - T\Delta S$), and the prediction of spontaneity.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Not covered — see Acids & Bases, Equilibrium) | — |
| **Semester 2** | Enthalpy, calorimetry, Hess's law, bond energies, $\Delta S$, $\Delta G$, spontaneity, standard formation enthalpies | Calculate $\Delta H$ from calorimetry/Hess/bond energies, compute $\Delta G$ and predict spontaneity, relate $\Delta G$ to $K$ |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| อุณหเคมี | Thermochemistry | Heat in chemical reactions |
| เอนทาลปี | Enthalpy | $H$ (kJ), heat at constant $P$ |
| การเปลี่ยนแปลงเอนทาลปี | Enthalpy change | $\Delta H$ |
| คายความร้อน | Exothermic | $\Delta H < 0$ |
| ดูดความร้อน | Endothermic | $\Delta H > 0$ |
| แคลอรีมิเตอร์ | Calorimeter | Measures heat |
| แคลอรีมิเตอร์แบบถ้วยกาแฟ | Coffee-cup calorimeter | Constant pressure |
| บอมบ์แคลอรีมิเตอร์ | Bomb calorimeter | Constant volume |
| ความจุความร้อน | Heat capacity | $C$ (J/K) |
| ความจุความร้อนจำเพาะ | Specific heat capacity | $c$ (J/g·K) |
| กฎของเฮสส์ | Hess's law | $\Delta H$ path-independent |
| เอนทาลปีการเกิดมาตรฐาน | Standard enthalpy of formation | $\Delta H_f^\circ$ |
| สถานะมาตรฐาน | Standard state | 1 atm, 25 °C, 1 M |
| พลังงานพันธะ | Bond energy | Energy to break 1 mol of bonds |
| เอนโทรปี | Entropy | $S$ (J/K), disorder |
| พลังงานกิ๊บส์อิสระ | Gibbs free energy | $G = H - TS$ |
| กระบวนการเกิดเองได้ | Spontaneous process | $\Delta G < 0$ |
| กระบวนการเกิดเองไม่ได้ | Non-spontaneous | $\Delta G > 0$ |
| สมดุล | Equilibrium | $\Delta G = 0$ |

---

## 3 | Key Concepts

### 3.1 Energy, Heat, and Enthalpy

The **First Law of Thermodynamics**: energy is neither created nor destroyed.
$$\Delta U = q + w$$
where $q$ is heat added to system, $w$ is work done on system.

**Enthalpy** is the heat content at constant pressure:
$$H = U + PV, \quad \Delta H = q_p$$
The change in enthalpy equals the heat absorbed/released at constant pressure (open beaker).

- $\Delta H < 0$: **exothermic** (heat released to surroundings, e.g. combustion).
- $\Delta H > 0$: **endothermic** (heat absorbed from surroundings, e.g. photosynthesis).

### 3.2 Calorimetry

**Coffee-cup calorimeter** (constant $P$, dilute aqueous):
$$q = mc\Delta T$$
where $m$ = mass of solution, $c$ = specific heat capacity (≈ 4.18 J/g·K for water), $\Delta T$ = temperature change.
$$q_{rxn} = -q_{soln} = -mc\Delta T$$

**Bomb calorimeter** (constant $V$, combustion):
$$q_{rxn} = -C_{cal}\Delta T$$
where $C_{cal}$ is the calorimeter constant (J/K), determined by burning a standard (e.g. benzoic acid).

### 3.3 Thermochemical Equations and Stoichiometry

Coefficients in thermochemical equations represent **moles**, so:
$$\ce{CH4(g) + 2O2(g) -> CO2(g) + 2H2O(l)} \quad \Delta H = -890\ \text{kJ}$$

Burning 2 mol of $\ce{CH4}$ releases 2 × 890 = 1780 kJ. Reversing the reaction reverses the sign of $\Delta H$.

### 3.4 Hess's Law

The total enthalpy change is **independent of the pathway** — it depends only on the initial and final states. Allows calculation of $\Delta H$ for reactions that are difficult to measure directly, by combining known reactions.

**Procedure:**
1. Write target reaction.
2. Manipulate given reactions (reverse → flip sign; multiply by $n$ → multiply $\Delta H$ by $n$) so they add up to target.
3. Sum enthalpies.

### 3.5 Standard Enthalpy of Formation ($\Delta H_f^\circ$)

$\Delta H_f^\circ$ = enthalpy change when 1 mol of a compound is formed from its elements in their standard states.
- $\Delta H_f^\circ$ for any element in its standard state = 0.
- $\Delta H_f^\circ$ for $\ce{H2O(l)} = -285.8$ kJ/mol.

**Calculation of $\Delta H_{rxn}^\circ$:**
$$\Delta H_{rxn}^\circ = \sum n \Delta H_f^\circ(\text{products}) - \sum n \Delta H_f^\circ(\text{reactants})$$

### 3.6 Bond Energies

Bond energy (BE) = average energy required to break 1 mol of a particular bond in the gas phase.
- **Breaking** a bond requires energy (+BE).
- **Forming** a bond releases energy (–BE).

$$\Delta H_{rxn} = \sum \text{BE(bonds broken)} - \sum \text{BE(bonds formed)}$$

This works because energy required to break reactants' bonds minus energy released forming products' bonds equals the net heat change.

### 3.7 Entropy ($\Delta S$)

Entropy is a measure of **disorder** or the number of microstates available to a system.
- Units: J/(mol·K) (note: J, not kJ).
- Gases > liquids > solids in entropy.
- More particles → higher entropy.
- Mixing increases entropy.

Second Law: the total entropy of universe always increases for a spontaneous process.

### 3.8 Gibbs Free Energy ($\Delta G$)

The maximum non-expansion work obtainable from a process at constant $T$ and $P$:
$$\Delta G = \Delta H - T\Delta S$$

| $\Delta H$ | $\Delta S$ | $\Delta G$ | Spontaneity |
|---|---|---|---|
| $-$ | $+$ | always $-$ | Always spontaneous |
| $+$ | $-$ | always $+$ | Never spontaneous |
| $-$ | $-$ | $-$ at low $T$ | Spontaneous at low $T$ |
| $+$ | $+$ | $-$ at high $T$ | Spontaneous at high $T$ |

### 3.9 $\Delta G$ and the Equilibrium Constant

$$\Delta G^\circ = -RT \ln K = -2.303 RT \log K$$

- $K > 1$: $\Delta G^\circ < 0$ (products favoured).
- $K < 1$: $\Delta G^\circ > 0$ (reactants favoured).
- $K = 1$: $\Delta G^\circ = 0$ (equal amounts).

This is the fundamental link between thermodynamics and equilibrium covered in Topic 09.

### 3.10 Temperature Dependence of Spontaneity

From $\Delta G = \Delta H - T\Delta S = 0$ at equilibrium:
$$T = \frac{\Delta H}{\Delta S}$$

Above this $T$, the sign of $\Delta G$ is set by $-\Delta S$; below, by $\Delta H$.

---

## 4 | Common Problem Types

### Type 1: Calorimetry
> Burning 1.50 g of $\ce{CH4}$ in a bomb calorimeter raises temperature by 13.3 °C. The calorimeter constant is 11.0 kJ/°C. Find $\Delta E$ per mole of $\ce{CH4}$.

**Solution:** $q = C_{cal}\Delta T = 11.0 \times 13.3 = 146.3$ kJ. Moles $\ce{CH4}$ = $1.50/16.04 = 0.0935$ mol.
$$\Delta E = \frac{-146.3}{0.0935} = -1565\ \text{kJ/mol}$$

### Type 2: Hess's law
> Given: (i) $\ce{N2(g) + O2(g) -> 2NO(g)} \quad \Delta H_1 = +180$ kJ
> (ii) $\ce{2NO(g) + O2(g) -> 2NO2(g)} \quad \Delta H_2 = -112$ kJ
> Find $\Delta H$ for $\ce{N2(g) + 2O2(g) -> 2NO2(g)}$.

**Solution:** Add (i) + (ii): $\Delta H = +180 + (-112) = +68$ kJ.

### Type 3: $\Delta H$ from standard formation enthalpies
> Find $\Delta H$ for $\ce{2C2H6(g) + 7O2(g) -> 4CO2(g) + 6H2O(l)}$.
> $\Delta H_f^\circ$: $\ce{C2H6} = -84.7$, $\ce{CO2} = -393.5$, $\ce{H2O(l)} = -285.8$ (all kJ/mol).

**Solution:**
$$\Delta H = [4(-393.5) + 6(-285.8)] - [2(-84.7) + 7(0)]$$
$$= [-1574.0 - 1714.8] - [-169.4] = -3288.8 + 169.4 = -3119\ \text{kJ}$$

### Type 4: $\Delta H$ from bond energies
> Estimate $\Delta H$ for $\ce{H2(g) + Cl2(g) -> 2HCl(g)}$.
> BE: H–H = 436, Cl–Cl = 242, H–Cl = 431 (kJ/mol).

**Solution:** Bonds broken: 1 H–H + 1 Cl–Cl = $436 + 242 = 678$ kJ.
Bonds formed: 2 H–Cl = $2 \times 431 = 862$ kJ.
$$\Delta H = 678 - 862 = -184\ \text{kJ}$$

### Type 5: $\Delta G$ and spontaneity
> $\Delta H = +125$ kJ, $\Delta S = +0.125$ kJ/K. At what $T$ does the reaction become spontaneous?

**Solution:** $\Delta G = 0$ at equilibrium:
$$T = \frac{\Delta H}{\Delta S} = \frac{125}{0.125} = 1000\ \text{K}$$
Above 1000 K, $\Delta G < 0$ (spontaneous).

### Type 6: $\Delta G^\circ$ from $K$
> At 25 °C, $K = 1.0 \times 10^{-5}$. Find $\Delta G^\circ$.

**Solution:** $R = 8.314 \times 10^{-3}$ kJ/(mol·K), $T = 298$ K.
$$\Delta G^\circ = -RT \ln K = -(8.314 \times 10^{-3})(298)\ln(10^{-5})$$
$$= -2.479 \times (-11.51) = +28.5\ \text{kJ/mol}$$

---

## 5 | Cross-Links

- [[05_Stoichiometry]] — mole ratios in thermochemical equations
- [[07_Gases]] — work $w = -P\Delta V$ in PV-work problems
- [[09_Chemical_Equilibrium]] — $\Delta G^\circ = -RT \ln K$ (thermodynamics ↔ equilibrium)
- [[12_Reaction_Kinetics]] — activation energy $E_a$ vs thermodynamic $\Delta H$
- [[02_Thermodynamics_and_Waves_-_Overview|Physics: Thermodynamics]] — First/Second/Third Laws
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — logarithms, exponentials
