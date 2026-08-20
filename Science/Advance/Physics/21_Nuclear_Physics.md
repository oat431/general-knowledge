---
tags:
  - physics
  - advance
  - nuclear-physics
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว303"]
---

# Nuclear Physics — ฟิสิกส์นิวเคลียร์

> *"The release of atomic energy has created a problem more grave than any ever faced by the human race."* — J. Robert Oppenheimer

Nuclear physics studies the nucleus — the dense core of the atom containing protons and neutrons. Despite occupying a tiny fraction of the atom's volume, the nucleus holds over 99.9% of its mass. The strong nuclear force binds nucleons together, while the electromagnetic force pushes protons apart. This interplay governs nuclear stability, radioactivity, fission, and fusion. The discovery of nuclear energy transformed both science and society, providing enormous power for both generation and destruction.

In the ว303 curriculum, students study nuclear structure, binding energy, the three types of radioactive decay, the radioactive decay law and half-life, nuclear fission and fusion, and the basic principles of nuclear energy production.

---

## 1 | Course Coverage

### ม.6 (ว303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Nuclear structure, isotopes, binding energy, mass defect, radioactive decay (α, β, γ), decay law, half-life | Calculate mass defect and binding energy; apply decay law $N = N_0 e^{-\lambda t}$; compute half-life and activity |
| **Semester 2** | Nuclear fission, nuclear fusion, chain reactions, nuclear reactors, radiation safety | Balance nuclear equations; explain fission vs fusion energy release; describe reactor basics and radiation units |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| นิวเคลียส | Nucleus | Central core of atom |
| นิวคลีออน | Nucleon | Proton or neutron |
| โปรตอน | Proton | $p$, charge +e, mass ~1.007 u |
| นิวตรอน | Neutron | $n$, charge 0, mass ~1.009 u |
| เลขมวลอะตอม | Mass number | $A = Z + N$ |
| เลขปรมาณู | Atomic number | $Z$, number of protons |
| ไอโซโทป | Isotope | Same Z, different N |
| ความบกพร่องมวล | Mass defect | $\Delta m$, converted to binding energy |
| พลังงานยึดเหนี่ยว | Binding energy | $E_B = \Delta m \, c^2$ |
| กัมมันตรังษี | Radioactivity | Spontaneous nuclear decay |
| สารกัมมันตรังษี | Radioactive substance | Undergoes decay |
| ประจุแอลฟา | Alpha particle | $_2^4\alpha$, He nucleus |
| อนุภาคเบตา | Beta particle | $\beta^-$ (electron) or $\beta^+$ (positron) |
| รังสีแกมมา | Gamma ray | High-energy photon |
| ครึ่งชีวิต | Half-life | $t_{1/2}$, time for half to decay |
| ค่าคงที่การสลาย | Decay constant | $\lambda = \ln 2 / t_{1/2}$ |
| กิจกรรม | Activity | $A = \lambda N$, measured in Bq |
| การแบ่งแยกนิวเคลียร์ | Nuclear fission | Heavy nucleus splits |
| การหลอมนิวเคลียร์ | Nuclear fusion | Light nuclei combine |
| ปฏิกิริยาลูกโซ่ | Chain reaction | Self-sustaining fission |
| บีเคเรล | Becquerel | Bq = 1 decay/s |

---

## 3 | Key Concepts

### 3.1 Nuclear Structure and Notation

A nucleus is described by its **atomic number** $Z$ (protons) and **mass number** $A$ (protons + neutrons), with neutron number $N = A - Z$. Standard notation:

$$\underset{Z}{^{A}}X$$

**Isotopes (ไอโซโทป)** are atoms with the same $Z$ but different $N$ — same element, different mass. For example: $^{1}$H, $^{2}$H (deuterium), $^{3}$H (tritium) are all hydrogen isotopes.

Nuclear radius scales as:

$$R = R_0 A^{1/3}, \quad R_0 \approx 1.2 \ \text{fm}$$

Nuclear density is roughly constant at $\sim 2.3 \times 10^{17}$ kg/m³ — extraordinarily dense.

### 3.2 Mass Defect and Binding Energy

The mass of a nucleus is always **less** than the sum of its individual nucleons. This **mass defect** $\Delta m$ is converted to binding energy:

$$E_B = \Delta m \, c^2$$

For a nucleus $\underset{Z}{^{A}}X$:

$$\Delta m = Z \, m_p + N \, m_n - M_{\text{nucleus}}$$

The **binding energy per nucleon** $E_B/A$ is a key measure of nuclear stability. It peaks around iron-56 ($\sim$8.8 MeV/nucleon), meaning:

- Nuclei lighter than Fe release energy via **fusion**
- Nuclei heavier than Fe release energy via **fission**

### 3.3 Radioactive Decay

Unstable nuclei decay by emitting radiation. Three primary types:

| Type | Emission | Change | Penetration |
|---|---|---|---|
| **Alpha (α)** | $_2^4\text{He}$ nucleus | $A \to A-4$, $Z \to Z-2$ | Low (stopped by paper) |
| **Beta minus (β⁻)** | $e^-$ + $\bar{\nu}$ | $Z \to Z+1$ | Medium (stopped by Al) |
| **Beta plus (β⁺)** | $e^+$ + $\nu$ | $Z \to Z-1$ | Medium |
| **Gamma (γ)** | Photon | No change in $A$ or $Z$ | High (needs Pb/concrete) |

Example of alpha decay:

$$^{238}_{92}\text{U} \to ^{234}_{90}\text{Th} + ^4_2\text{He}$$

Example of beta-minus decay:

$$^{14}_{6}\text{C} \to ^{14}_{7}\text{N} + e^- + \bar{\nu}$$

### 3.4 Decay Law and Half-Life

Radioactive decay is a statistical, first-order process. The number of undecayed nuclei decreases exponentially:

$$N(t) = N_0 \, e^{-\lambda t}$$

where $\lambda$ is the **decay constant**. The **half-life** (ครึ่งชีวิต) is:

$$t_{1/2} = \frac{\ln 2}{\lambda} \approx \frac{0.693}{\lambda}$$

The **activity** (กิจกรรม), or decay rate, is:

$$A = \left|\frac{dN}{dt}\right| = \lambda N = \lambda N_0 e^{-\lambda t}$$

Activity is measured in **becquerels (Bq)**, where 1 Bq = 1 decay per second. Another common unit is the **curie (Ci)**: $1 \ \text{Ci} = 3.7 \times 10^{10}$ Bq.

After $n$ half-lives: $N/N_0 = (1/2)^n$.

### 3.5 Nuclear Fission

In **nuclear fission** (การแบ่งแยกนิวเคลียร์), a heavy nucleus (e.g., $^{235}$U) absorbs a neutron and splits into two lighter nuclei (fission fragments), releasing several neutrons and ~200 MeV of energy:

$$^{235}_{92}\text{U} + n \to ^{141}_{56}\text{Ba} + ^{92}_{36}\text{Kr} + 3n + \text{energy}$$

The released neutrons can trigger further fissions, creating a **chain reaction (ปฏิกิริยาลูกโซ่)**. In a nuclear reactor, control rods (e.g., cadmium, boron) absorb excess neutrons to maintain a controlled chain reaction.

### 3.6 Nuclear Fusion

In **nuclear fusion** (การหลอมนิวเคลียร์), light nuclei combine to form a heavier nucleus, releasing energy. The proton-proton chain in the Sun:

$$4 \, ^1\text{H} \to ^4\text{He} + 2e^+ + 2\nu + \text{energy} \ (\sim 26.7 \ \text{MeV})$$

Fusion releases more energy per unit mass than fission and produces no long-lived radioactive waste, but requires extremely high temperatures ($\sim 10^8$ K) to overcome Coulomb repulsion — which is why controlled fusion for power generation remains technologically challenging.

---

## 4 | Common Problem Types

### Type 1: Mass defect and binding energy
> Find the binding energy of $^4_2$He given: $m_p = 1.0073$ u, $m_n = 1.0087$ u, $M_{\text{He}} = 4.0026$ u.

**Solution:**

$$\Delta m = 2m_p + 2m_n - M_{\text{He}} = 2(1.0073) + 2(1.0087) - 4.0026$$

$$\Delta m = 2.0146 + 2.0174 - 4.0026 = 0.0294 \ \text{u}$$

Using $1 \ \text{u} = 931.5$ MeV/$c^2$:

$$E_B = 0.0294 \times 931.5 \approx 27.4 \ \text{MeV}$$

$$\frac{E_B}{A} = \frac{27.4}{4} \approx 6.85 \ \text{MeV/nucleon}$$

---

### Type 2: Half-life calculation
> A radioactive sample has an activity of 8000 Bq. After 30 days, the activity is 1000 Bq. Find the half-life and decay constant.

**Solution:**

$$\frac{A}{A_0} = \frac{1000}{8000} = \frac{1}{8} = \left(\frac{1}{2}\right)^3$$

So 30 days = 3 half-lives → $t_{1/2} = 10$ days.

$$\lambda = \frac{\ln 2}{t_{1/2}} = \frac{0.693}{10 \times 86400} \approx 8.02 \times 10^{-7} \ \text{s}^{-1}$$

---

### Type 3: Balancing nuclear equations
> Balance: $^{238}_{92}\text{U} \to ^{206}_{82}\text{Pb} + ?$

**Solution:**

Change in $A$: $238 - 206 = 32$, so 8 alpha decays (each reduces $A$ by 4).
Change in $Z$: $92 - 8(2) = 76$, but final $Z = 82$, so $82 - 76 = 6$ beta-minus decays needed.

$$^{238}_{92}\text{U} \to ^{206}_{82}\text{Pb} + 8 \, ^4_2\text{He} + 6 \, e^- + 6 \, \bar{\nu}$$

---

### Type 4: Energy from fission
> How many $^{235}$U fissions are needed to produce 1 MW of power for one day? (Assume 200 MeV per fission.)

**Solution:**

Energy needed: $E = P \times t = 10^6 \times 86400 = 8.64 \times 10^{13}$ J

Energy per fission: $200 \ \text{MeV} = 200 \times 1.6 \times 10^{-13} = 3.2 \times 10^{-11}$ J

$$N = \frac{8.64 \times 10^{13}}{3.2 \times 10^{-11}} \approx 2.7 \times 10^{24} \ \text{fissions}$$

Mass consumed: $\frac{2.7 \times 10^{24}}{6.022 \times 10^{23}} \times 235 \approx 1.05$ kg of $^{235}$U. ✓

---

## 5 | Cross-Links

- [[18_Special_Relativity]] — Mass-energy equivalence $E = mc^2$ is the basis of binding energy
- [[20_Atomic_Physics]] — Nuclear structure determines the atom's identity; radioactive decay changes elements
- [[19_Quantum_Physics]] — Quantum tunneling explains alpha decay and fusion barrier penetration
- [[23_Astrophysics_and_Cosmology]] — Nuclear fusion powers stars; nucleosynthesis creates elements
