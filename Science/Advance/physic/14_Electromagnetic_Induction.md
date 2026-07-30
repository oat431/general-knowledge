---
tags:
  - physics
  - advance
  - electromagnetic-induction
  - induction
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Electromagnetic Induction — การเหนี่ยวนำแม่เหล็กไฟฟ้า

> *"The most beautiful and important discoveries in physics have been made by following the clue of analogy."* — Michael Faraday

Electromagnetic induction is the generation of an electromotive force (EMF) by a changing magnetic flux. Faraday's law quantifies this relationship, and Lenz's law determines the direction of the induced current — always opposing the change that produced it. This principle underlies generators, transformers, inductors, and the entire technology of electrical power. Inductance is the magnetic analog of capacitance, and together they form the LC circuits central to AC theory.

In ว302 Semester 2, students connect the static electricity and magnetism of Semester 1 to dynamic systems. Generators convert mechanical energy to electrical energy, while transformers step voltages up and down for efficient power transmission. AC circuit analysis introduces impedance, resonant frequency, and the power factor — concepts essential to all modern electrical engineering.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Magnetism foundations) | — |
| **Semester 2** | Faraday's law, Lenz's law, generators, transformers, inductance, AC circuits, RLC | Apply Faraday's & Lenz's laws; transformer calculations; AC impedance; resonance |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| การเหนี่ยวนำแม่เหล็กไฟฟ้า | Electromagnetic induction | Changing flux → EMF |
| กฎของฟาราเดย์ | Faraday's law | $\mathcal{E} = -N\frac{d\Phi_B}{dt}$ |
| กฎของเลนซ์ | Lenz's law | Induced current opposes change |
| ฟลักซ์แม่เหล็ก | Magnetic flux | $\Phi_B = BA\cos\theta$ (Wb) |
| การเหนี่ยวนำตนเอง | Self-inductance | $L$ (H) |
| การเหนี่ยวนำร่วม | Mutual inductance | $M$ (H) |
| เครื่องกำเนิดไฟฟ้า | Generator | Mechanical → electrical |
| หม้อแปลงไฟฟ้า | Transformer | $V_s/V_p = N_s/N_p$ |
| ไฟฟ้ากระแสสลับ | Alternating current (AC) | $V = V_0\sin\omega t$ |
| ความต้านทานเชิงต้าน | Impedance | $Z$ ($\Omega$) |
| ความถี่เรโซแนนซ์ | Resonant frequency | $f_0 = \frac{1}{2\pi\sqrt{LC}}$ |
| ตัวเหนี่ยวนำ | Inductor | $L$ (H) |

---

## 3 | Key Concepts

### 3.1 Magnetic Flux

$$\Phi_B = \vec{B}\cdot\vec{A} = BA\cos\theta$$

Where $\theta$ is the angle between $\vec{B}$ and the area normal. Flux is maximized when $\vec{B}$ is perpendicular to the surface.

### 3.2 Faraday's Law

Induced EMF equals the negative rate of change of flux:

$$\mathcal{E} = -N\frac{d\Phi_B}{dt}$$

For a motional EMF (rod of length $L$ moving at velocity $v$ perpendicular to $B$):

$$\mathcal{E} = BLv$$

### 3.3 Lenz's Law

The direction of the induced current opposes the change in magnetic flux that produced it. This is a consequence of energy conservation — the law appears as the negative sign in Faraday's law.

### 3.4 Inductance

**Self-inductance:** $\mathcal{E} = -L\frac{dI}{dt}$

For a solenoid: $L = \mu_0 n^2 A l = \mu_0 N^2 A / l$

**Energy stored in an inductor:** $U = \frac{1}{2}LI^2$

**Mutual inductance:** $\mathcal{E}_2 = -M\frac{dI_1}{dt}$

### 3.5 Generators

A coil rotating in a magnetic field produces sinusoidal EMF:

$$\mathcal{E} = NBA\omega\sin(\omega t)$$

Where $\omega$ is angular frequency. This is the basis of AC power generation.

### 3.6 Transformers

$$\frac{V_s}{V_p} = \frac{N_s}{N_p}, \qquad \frac{I_s}{I_p} = \frac{N_p}{N_s}$$

For an ideal transformer (100% efficiency): $V_p I_p = V_s I_s$.

Step-up: $N_s > N_p$ (increases voltage, decreases current). Step-down: $N_s < N_p$.

### 3.7 AC Circuits and Impedance

For an RLC series circuit with AC source $V = V_0\sin\omega t$:

$$Z = \sqrt{R^2 + (X_L - X_C)^2}$$

Where $X_L = \omega L$ (inductive reactance) and $X_C = 1/(\omega C)$ (capacitive reactance).

RMS values: $V_{\text{rms}} = V_0/\sqrt{2}$, $I_{\text{rms}} = I_0/\sqrt{2}$.

Power: $P_{\text{avg}} = V_{\text{rms}} I_{\text{rms}} \cos\phi$ where $\cos\phi = R/Z$ is the power factor.

**Resonance:** $f_0 = \frac{1}{2\pi\sqrt{LC}}$, at which $Z = R$ (minimum impedance, maximum current).

---

## 4 | Common Problem Types

### Type 1: Faraday's Law
> A coil of 100 turns has its flux change from 0.05 Wb to 0.02 Wb in 0.1 s. Find the induced EMF.

**Solution:**

$$\mathcal{E} = -N\frac{\Delta\Phi}{\Delta t} = -100\frac{0.02 - 0.05}{0.1} = 30 \text{ V}$$

### Type 2: Transformer
> A transformer has 500 primary turns and 5000 secondary turns. If $V_p = 220$ V, find $V_s$.

**Solution:**

$$V_s = V_p \frac{N_s}{N_p} = 220 \times \frac{5000}{500} = 2200 \text{ V}$$

### Type 3: Motional EMF
> A 0.5 m rod moves at 4 m/s perpendicular to a 0.8 T field. Find the induced EMF.

**Solution:**

$$\mathcal{E} = BLv = (0.8)(0.5)(4) = 1.6 \text{ V}$$

### Type 4: Inductor Energy
> A 20 mH inductor carries 5 A. Find the stored energy.

**Solution:**

$$U = \frac{1}{2}LI^2 = \frac{1}{2}(0.02)(5)^2 = 0.25 \text{ J}$$

### Type 5: AC Resonance
> An RLC circuit has $L = 10$ mH and $C = 100\,\mu\text{F}$. Find the resonant frequency.

**Solution:**

$$f_0 = \frac{1}{2\pi\sqrt{LC}} = \frac{1}{2\pi\sqrt{(0.01)(100 \times 10^{-6})}} = 159 \text{ Hz}$$

---

## 5 | Cross-Links

- [[11_Electrostatics]] — Capacitors in AC circuits provide capacitive reactance
- [[12_Electric_Circuits]] — Ohm's law generalizes to impedance in AC
- [[13_Magnetism]] — Magnetic fields and flux are the foundation of induction
- [[15_Electromagnetic_Waves]] — LC oscillations radiate as EM waves
- [[10_Heat_and_Thermodynamics]] — Power plants are heat engines driving generators
