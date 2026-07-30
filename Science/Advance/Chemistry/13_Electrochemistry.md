---
tags:
  - chemistry
  - advance
  - electrochemistry
  - ipst
source: "IPST (สสวท.) Chemistry Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว312"]
---

# Electrochemistry — เคมีไฟฟ้า

> *"A redox reaction is an argument over electrons; electrochemistry is the court that decides who wins."* — Adapted from electrochemistry

Electrochemistry is the study of the relationship between chemical energy and electrical energy. It is the third and final topic of Semester 2 in ว312, and it draws together everything from the previous twelve topics — atomic structure, bonding, equilibrium, thermodynamics, kinetics, and acid–base chemistry — to explain how batteries generate current, how metals corrode, and how we can plate one metal onto another.

This note covers oxidation–reduction (redox) reactions, half-reactions and balancing redox equations, galvanic (voltaic) cells, standard electrode potentials ($E^\circ$), cell potential, the Nernst equation, electrolysis, Faraday's laws of electrolysis, and corrosion.

---

## 1 | Course Coverage

### ม.5 (ว312)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Not covered — see Acids & Bases, Equilibrium) | — |
| **Semester 2** | Redox, half-reactions, balancing redox (acidic/basic), galvanic cells, standard electrode potentials, cell potential, Nernst equation, electrolysis, Faraday's laws, corrosion | Assign oxidation numbers, balance redox, identify anode/cathode, calculate $E^\circ_{cell}$, apply Nernst, calculate mass deposited in electrolysis |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| เคมีไฟฟ้า | Electrochemistry | Chemical ↔ electrical energy |
| ปฏิกิริยารีดอกซ์ | Redox reaction | Electron transfer |
| ออกซิเดชัน | Oxidation | Loss of electrons (OIL) |
| รีดักชัน | Reduction | Gain of electrons (RIG) |
| เลขออกซิเดชัน | Oxidation number | Charge tracking |
| ตัวออกซิไดซ์ | Oxidizing agent | Gets reduced |
| ตัวรีดิวซ์ | Reducing agent | Gets oxidized |
| ปฏิกิริยาครึ่ง | Half-reaction | Oxidation or reduction alone |
| เซลล์กัลวานิก | Galvanic / voltaic cell | Spontaneous, produces current |
| เซลล์อิเล็กโทรไลต์ | Electrolytic cell | Non-spontaneous, requires current |
| แอโนด | Anode | Oxidation |
| แคโทด | Cathode | Reduction |
| ค่าศักย์ไฟฟ้ามาตรฐาน | Standard electrode potential | $E^\circ$ (V) |
| ขั้วไฟฟ้าไฮโดรเจนมาตรฐาน | Standard hydrogen electrode (SHE) | $E^\circ = 0$ V reference |
| แรงเคลื่อนไฟฟ้าเซลล์ | Cell potential | $E_{cell}$ (V) |
| สะพานเกลือ | Salt bridge | Maintains charge balance |
| สมการเนิร์นสต์ | Nernst equation | $E = E^\circ - (RT/nF)\ln Q$ |
| การอิเล็กโทรไลซิส | Electrolysis | Current drives reaction |
| กฎของฟาราเดย์ | Faraday's laws | $m = (Q/F)(M/n)$ |
| ค่าคงที่ฟาราเดย์ | Faraday constant | $F = 96\,485$ C/mol e⁻ |
| การกัดกร่อน | Corrosion | Unwanted redox (e.g. rusting) |
| การป้องกันการกัดกร่อน | Cathodic protection | Sacrificial anode |
| เซลล์เชื้อเพลิง | Fuel cell | Continuous galvanic cell |

---

## 3 | Key Concepts

### 3.1 Oxidation Numbers

Rules:
1. Element in standard state: 0 (e.g. $\ce{O2}$, $\ce{Fe}$, $\ce{Cl2}$).
2. Monatomic ion: equal to its charge.
3. F always −1 in compounds.
4. O usually −2 (except in peroxides −1, superoxides −½).
5. H usually +1 (except in metal hydrides, −1).
6. Sum of oxidation numbers in a neutral compound = 0; in a polyatomic ion = ion charge.

### 3.2 Balancing Redox Equations

**Half-reaction method (acidic solution):**
1. Separate into oxidation and reduction half-reactions.
2. Balance atoms other than O and H.
3. Balance O by adding $\ce{H2O}$, then H by adding $\ce{H+}$.
4. Balance charge by adding electrons.
5. Multiply half-reactions so electrons cancel.
6. Add and simplify.

**Example:** $\ce{MnO4- + Fe^2+ -> Mn^2+ + Fe^3+}$ (acidic)
- Reduction: $\ce{MnO4- + 8H+ + 5e- -> Mn^2+ + 4H2O}$
- Oxidation: $\ce{Fe^2+ -> Fe^3+ + e-}$ (×5)
- Overall: $\ce{MnO4- + 5Fe^2+ + 8H+ -> Mn^2+ + 5Fe^3+ + 4H2O}$

**Basic solution:** Same procedure, then add $\ce{OH-}$ to both sides to neutralize $\ce{H+}$, forming $\ce{H2O}$.

### 3.3 Galvanic (Voltaic) Cells

A spontaneous redox reaction ($\Delta G < 0$, $E_{cell} > 0$) is harnessed to produce electrical energy. The two half-reactions occur in separate **half-cells** connected by a wire (electrons flow) and a **salt bridge** (ions flow to maintain charge balance).

- **Anode** (oxidation) — negative terminal in galvanic cell
- **Cathode** (reduction) — positive terminal
- Electrons flow anode → cathode through external circuit

**Cell notation** (anode on left):
$$\ce{Zn(s) | Zn^2+(aq) || Cu^2+(aq) | Cu(s)}$$

### 3.4 Standard Electrode Potential ($E^\circ$)

The **standard hydrogen electrode (SHE)** is the reference:
$$\ce{2H+(aq, 1 M) + 2e- -> H2(g, 1 atm)} \quad E^\circ = 0\ \text{V}$$

For any half-cell:
$$\text{Half-cell} \quad | \quad E^\circ \text{ (V)}$$

Selected standard reduction potentials (more positive = stronger oxidizer, more negative = stronger reducer):

| Half-reaction | $E^\circ$ (V) |
|---|---|
| $\ce{F2 + 2e- -> 2F-}$ | +2.87 |
| $\ce{Au^3+ + 3e- -> Au}$ | +1.50 |
| $\ce{Cl2 + 2e- -> 2Cl-}$ | +1.36 |
| $\ce{O2 + 4H+ + 4e- -> 2H2O}$ | +1.23 |
| $\ce{Ag+ + e- -> Ag}$ | +0.80 |
| $\ce{Cu^2+ + 2e- -> Cu}$ | +0.34 |
| $\ce{2H+ + 2e- -> H2}$ | 0.00 |
| $\ce{Pb^2+ + 2e- -> Pb}$ | −0.13 |
| $\ce{Fe^2+ + 2e- -> Fe}$ | −0.44 |
| $\ce{Zn^2+ + 2e- -> Zn}$ | −0.76 |
| $\ce{Al^3+ + 3e- -> Al}$ | −1.66 |
| $\ce{Mg^2+ + 2e- -> Mg}$ | −2.37 |
| $\ce{Li+ + e- -> Li}$ | −3.04 |

### 3.5 Cell Potential

For a galvanic cell:
$$E^\circ_{cell} = E^\circ_{cathode} - E^\circ_{anode}$$
(both as reduction potentials).

If $E^\circ_{cell} > 0$, the reaction is **spontaneous** under standard conditions.

**Activity series:** metals higher in the series (more negative $E^\circ$) are stronger reducing agents and displace metals below them from solution.

### 3.6 Nernst Equation

For non-standard conditions:
$$E_{cell} = E^\circ_{cell} - \frac{RT}{nF}\ln Q = E^\circ_{cell} - \frac{0.0592}{n}\log Q \quad (\text{at 25 °C})$$

where $n$ is moles of electrons transferred in the balanced equation, $Q$ is the reaction quotient.

Concentration cells ($E^\circ_{cell} = 0$): $E = -\frac{0.0592}{n}\log Q$.

### 3.7 Electrolysis

In an **electrolytic cell**, an external power source drives a non-spontaneous reaction.
- **Anode**: still oxidation (now connected to + terminal of source).
- **Cathode**: still reduction (connected to − terminal).
- Cations migrate to cathode, anions to anode.

**Faraday's First Law:** The mass of substance liberated is proportional to the charge passed.
**Faraday's Second Law:** For the same charge, mass is proportional to equivalent weight ($M/n$).

Combined:
$$m = \frac{Q \cdot M}{n \cdot F} = \frac{I \cdot t \cdot M}{n \cdot F}$$
where $m$ = mass (g), $I$ = current (A), $t$ = time (s), $M$ = molar mass, $n$ = electrons per atom/ion, $F = 96\,485$ C/mol.

### 3.8 Corrosion

**Rusting of iron** is an electrochemical process:
- Anode: $\ce{Fe -> Fe^2+ + 2e-}$
- Cathode: $\ce{O2 + 2H2O + 4e- -> 4OH-}$

Forms porous $\ce{Fe(OH)2}$, which oxidizes further to hydrated $\ce{Fe2O3}$ (rust). Requires water, oxygen, and electrolyte.

**Prevention:**
- Painting/coating (barrier)
- Galvanizing (Zn coating — Zn is sacrificial anode)
- Cathodic protection (attach a more active metal like Mg, Zn as sacrificial anode)
- Alloying (stainless steel: Fe + Cr + Ni — Cr forms passive oxide layer)
- Tin plating (cathodic protection only if scratched through to Fe)

---

## 4 | Common Problem Types

### Type 1: Balance redox (acidic)
> Balance $\ce{Cr2O7^2- + C2H5OH -> Cr^3+ + CH3COOH}$ (acidic).

**Solution:** Half-reactions
- Reduction: $\ce{Cr2O7^2- + 14H+ + 6e- -> 2Cr^3+ + 7H2O}$
- Oxidation: $\ce{C2H5OH + H2O -> CH3COOH + 4H+ + 4e-}$ (×3/2 or ×1.5)
- Multiply: reduction by 2, oxidation by 3 → 12 e⁻ each
$$2\ce{Cr2O7^2-} + 3\ce{C2H5OH} + 16\ce{H+} -> 4\ce{Cr^3+} + 3\ce{CH3COOH} + 11\ce{H2O}$$

### Type 2: Calculate $E^\circ_{cell}$
> For $\ce{Zn + Cu^2+ -> Zn^2+ + Cu}$, find $E^\circ_{cell}$.

**Solution:**
- Cathode (reduction): $\ce{Cu^2+ + 2e- -> Cu}$, $E^\circ = +0.34$ V
- Anode (oxidation): $\ce{Zn -> Zn^2+ + 2e-}$, $E^\circ_{red} = -0.76$ V
$$E^\circ_{cell} = 0.34 - (-0.76) = +1.10\ \text{V}$$

### Type 3: Spontaneity from $E^\circ$
> Is $\ce{Fe + 2Ag+ -> Fe^2+ + 2Ag}$ spontaneous?

**Solution:**
- Cathode: $\ce{Ag+ + e- -> Ag}$, $E^\circ = +0.80$ V
- Anode: $\ce{Fe^2+ + 2e- -> Fe}$, $E^\circ = -0.44$ V
$$E^\circ_{cell} = 0.80 - (-0.44) = +1.24\ \text{V} > 0$$
**Spontaneous.** Yes, Fe displaces Ag.

### Type 4: Nernst equation
> For the Daniell cell ($\ce{Zn|Zn^2+||Cu^2+|Cu}$), $[\ce{Zn^2+}] = 0.10$ M, $[\ce{Cu^2+}] = 1.0$ M, $E^\circ = 1.10$ V. Find $E$.

**Solution:** $n = 2$, $Q = [\ce{Zn^2+}]/[\ce{Cu^2+}] = 0.10$.
$$E = 1.10 - \frac{0.0592}{2}\log(0.10) = 1.10 - 0.0296 \times (-1) = 1.10 + 0.030 = 1.13\ \text{V}$$

### Type 5: Faraday's law — mass deposited
> How many grams of $\ce{Cu}$ are deposited by passing 5.0 A for 1.0 hour through $\ce{CuSO4}$ solution?

**Solution:** $Q = It = 5.0 \times 3600 = 18\,000$ C.
$\ce{Cu^2+ + 2e- -> Cu}$, $M_{Cu} = 63.5$, $n = 2$.
$$m = \frac{Q \cdot M}{n \cdot F} = \frac{18\,000 \times 63.5}{2 \times 96\,485} = 5.92\ \text{g}$$

### Type 6: Corrosion prevention
> An underground iron pipe is connected to a magnesium rod. Which corrodes, and why?

**Solution:** Mg is more active (more negative $E^\circ$, $-2.37$ V vs Fe $-0.44$ V). Mg acts as sacrificial anode and oxidizes preferentially, protecting the iron. This is **cathodic protection**.

---

## 5 | Cross-Links

- [[01_Atomic_Structure]] — electron configurations underlying redox behaviour
- [[02_Periodic_Table]] — activity series follows periodic trends
- [[05_Stoichiometry]] — mole calculations in Faraday's law
- [[07_Gases]] — gas electrodes (SHE, $\ce{Cl2/Cl-}$)
- [[08_Acids_and_Bases]] — pH electrodes; Nernst equation for $[\ce{H+}]$
- [[09_Chemical_Equilibrium]] — $E^\circ = (RT/nF)\ln K$
- [[11_Thermochemistry]] — $\Delta G^\circ = -nFE^\circ_{cell}$ (thermodynamics ↔ electrochemistry)
- [[12_Reaction_Kinetics]] — rate of electron transfer (Butler-Volmer)
- [[18_Biochemistry|Biology]] — biological electron transport, ATP synthesis
- [[02_Thermodynamics_and_Waves_-_Overview|Physics]] — circuits, potential, current
