---
tags:
  - physics
  - advance
  - circuits
  - electricity
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Electric Circuits — วงจรไฟฟ้า

> *"Nothing is too wonderful to be true, if it be consistent with the laws of nature."* — Michael Faraday

Electric circuits are pathways through which electric current flows, driven by a potential difference (voltage). The analysis of circuits rests on Ohm's law and Kirchhoff's rules, which encode the conservation of charge and energy. Resistors combine in series and parallel to form equivalent resistances. Capacitors introduce time-dependent behavior through RC circuits, and the concept of electrical power quantifies the rate of energy dissipation or transfer.

In the ว302 curriculum, students move from the static charge picture of electrostatics to the dynamic flow of current. Circuit analysis is one of the most practically applicable topics in physics — it underlies all electronic devices, power distribution, and electrical engineering. Mastery of Kirchhoff's laws enables the analysis of arbitrarily complex networks.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Ohm's law, series/parallel circuits, Kirchhoff's laws, RC circuits, electrical power | Calculate equivalent resistance; apply Kirchhoff's rules; analyze RC transients; compute power |
| **Semester 2** | (Continued in AC circuits, EM induction) | — |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| กระแสไฟฟ้า | Electric current | $I$ (A) |
| แรงดันไฟฟ้า | Voltage / EMF | $V$ or $\mathcal{E}$ (V) |
| ความต้านทาน | Resistance | $R$ ($\Omega$) |
| กฎของโอห์ม | Ohm's law | $V = IR$ |
| กฎของเคิร์ชฮอฟฟ์ | Kirchhoff's laws | KCL, KVL |
| อนุกรม | Series | Same $I$, voltages add |
| ขนาน | Parallel | Same $V$, currents add |
| ความต้านทานเทียบเท่า | Equivalent resistance | $R_{\text{eq}}$ |
| พลังงานไฟฟ้า | Electrical power | $P = VI$ (W) |
| ตัวเก็บประจุในวงจร | Capacitor in circuit | $C$ (F) |
| วงจร RC | RC circuit | $\tau = RC$ |
| แรงเคลื่อนไฟฟ้า | Electromotive force | $\mathcal{E}$ (V) |
| ความต้านทานภายใน | Internal resistance | $r$ ($\Omega$) |

---

## 3 | Key Concepts

### 3.1 Ohm's Law

$$V = IR$$

Where $V$ is voltage across, $I$ is current through, and $R$ is resistance. Ohm's law applies to ohmic (linear) materials. Resistance depends on material:

$$R = \rho\frac{L}{A}$$

Where $\rho$ is resistivity, $L$ is length, $A$ is cross-sectional area.

### 3.2 Series and Parallel Resistors

**Series:** $R_{\text{eq}} = R_1 + R_2 + \cdots$ — same current, voltages add.

**Parallel:** $\frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots$ — same voltage, currents add.

For two resistors in parallel: $R_{\text{eq}} = \frac{R_1 R_2}{R_1 + R_2}$.

### 3.3 Kirchhoff's Laws

**Kirchhoff's Current Law (KCL):** Sum of currents entering a node = sum leaving. (Conservation of charge.)

$$\sum I_{\text{in}} = \sum I_{\text{out}}$$

**Kirchhoff's Voltage Law (KVL):** Sum of voltages around any closed loop = 0. (Conservation of energy.)

$$\sum V_i = 0$$

### 3.4 EMF and Internal Resistance

A real battery has internal resistance $r$:

$$V_{\text{terminal}} = \mathcal{E} - Ir$$

Maximum current (short circuit): $I_{\text{max}} = \mathcal{E}/r$.

### 3.5 Electrical Power

$$P = VI = I^2R = \frac{V^2}{R}$$

Power dissipated as heat in a resistor (Joule heating). Energy: $E = Pt$.

### 3.6 RC Circuits

Charging a capacitor through resistor $R$:

$$Q(t) = Q_{\text{max}}\left(1 - e^{-t/\tau}\right), \quad \tau = RC$$

Discharging:

$$Q(t) = Q_0 \, e^{-t/\tau}$$

After one time constant $\tau$, the charge reaches $1 - 1/e \approx 63\%$ of maximum (charging) or drops to $1/e \approx 37\%$ (discharging).

---

## 4 | Common Problem Types

### Type 1: Equivalent Resistance
> Find $R_{\text{eq}}$ for $6\,\Omega$ and $3\,\Omega$ in parallel, then in series with $4\,\Omega$.

**Solution:**

$$R_{\text{parallel}} = \frac{6 \times 3}{6 + 3} = 2\,\Omega$$

$$R_{\text{eq}} = 2 + 4 = 6\,\Omega$$

### Type 2: Kirchhoff's Laws
> A loop has a 12 V battery and two resistors $4\,\Omega$ and $2\,\Omega$ in series. Find the current.

**Solution:** KVL: $12 - 4I - 2I = 0$, so $6I = 12$, $I = 2$ A.

### Type 3: Power Dissipation
> A $10\,\Omega$ resistor carries 2 A. Find the power dissipated.

**Solution:**

$$P = I^2R = (2)^2(10) = 40 \text{ W}$$

### Type 4: RC Time Constant
> A $100\,\mu\text{F}$ capacitor charges through a $50\,\text{k}\Omega$ resistor. Find $\tau$.

**Solution:**

$$\tau = RC = (50 \times 10^3)(100 \times 10^{-6}) = 5 \text{ s}$$

After 5 s, the capacitor is 63% charged.

---

## 5 | Cross-Links

- [[11_Electrostatics]] — Capacitors store energy; potential difference drives current
- [[13_Magnetism]] — Currents produce magnetic fields
- [[14_Electromagnetic_Induction]] — Changing currents induce EMF (inductors)
- [[14_Energy]] — Power is the rate of energy transfer
