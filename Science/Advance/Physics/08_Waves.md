---
tags:
  - physics
  - advance
  - waves
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Waves — คลื่น

> *"The ripples of a single stone carry the story of the entire pond."* — Adapted from wave theory

Waves (คลื่น) are disturbances that transfer energy from one point to another without transferring matter. They arise from oscillating sources — every wave is, at its heart, a connected chain of simple harmonic oscillators. Understanding waves unifies a vast range of phenomena: sound, light, water ripples, seismic waves, and even the quantum mechanical behaviour of matter. This topic concludes Semester 2 of the ว301 curriculum and builds directly on the study of oscillations.

This note covers wave properties (amplitude, wavelength, frequency, period, speed), types of waves (transverse and longitudinal), the wave equation, the principle of superposition, interference, standing waves, resonance in strings and pipes, and beat frequency.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Not covered — this is Semester 2 content) | — |
| **Semester 2** | Wave properties, transverse/longitudinal waves, wave equation, superposition, standing waves, resonance, beats | Apply $v = f\lambda$, solve standing wave problems in strings and pipes, compute beat frequency |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| คลื่น | Wave | Energy transfer |
| คลื่นตามขวาง | Transverse wave | Oscillation $\perp$ to propagation |
| คลื่นตามยาว | Longitudinal wave | Oscillation $\parallel$ to propagation |
| แอมพลิจูด | Amplitude | $A$ (m) |
| ความยาวคลื่น | Wavelength | $\lambda$ (m) |
| คาบ | Period | $T$ (s) |
| ความถี่ | Frequency | $f$ (Hz) |
| ความเร็วคลื่น | Wave speed | $v$ (m/s) |
| การซ้อนทับ | Superposition | Add displacements |
| การแทรกสอด | Interference | Constructive / destructive |
| คลื่นนิ่ง | Standing wave | Nodes and antinodes |
| จุดตัด | Node | Zero amplitude |
| จุดปลายสุด | Antinode | Maximum amplitude |
| การสาเรซอนานซ์ | Resonance | Natural frequency matching |
| ความถี่การตบ | Beat frequency | $f_{beat} = |f_1 - f_2|$ |
| สะท้อน | Reflection | Wave bounces back |

---

## 3 | Key Concepts

### 3.1 Wave Properties

A wave is described by:
- **Amplitude** ($A$): maximum displacement from equilibrium
- **Wavelength** ($\lambda$): distance between consecutive points in phase
- **Period** ($T$): time for one complete oscillation
- **Frequency** ($f$): number of oscillations per second ($f = 1/T$)

**The wave equation:**
$$v = f\lambda$$

### 3.2 Types of Waves

| Type | Direction of oscillation | Examples |
|---|---|---|
| Transverse (คลื่นตามขวาง) | Perpendicular to propagation | Light, string waves, water surface |
| Longitudinal (คลื่นตามยาว) | Parallel to propagation | Sound, seismic P-waves |

### 3.3 Wave Equation (Travelling Wave)

A sinusoidal wave travelling in the +x direction:
$$y(x,t) = A\sin(kx - \omega t + \phi)$$

where:
- $k = \frac{2\pi}{\lambda}$ is the **wave number**
- $\omega = 2\pi f$ is the **angular frequency**
- $\phi$ is the phase constant

Wave speed: $v = \frac{\omega}{k}$.

### 3.4 Superposition Principle

When two or more waves overlap, the resultant displacement is the sum of individual displacements:

$$y_{total} = y_1 + y_2$$

**Constructive interference:** waves in phase, amplitudes add ($\Delta \phi = 0, 2\pi, ...$).
**Destructive interference:** waves out of phase, amplitudes cancel ($\Delta \phi = \pi, 3\pi, ...$).

### 3.5 Standing Waves

A standing wave forms when two waves of equal amplitude and frequency travel in opposite directions (e.g. reflection at a fixed end). The result has **nodes** (points of zero amplitude) and **antinodes** (points of maximum amplitude).

**String fixed at both ends:**
$$L = n\frac{\lambda_n}{2}, \quad n = 1, 2, 3, \ldots$$
$$f_n = \frac{nv}{2L}$$

Harmonics: $f_1$ (fundamental), $f_2 = 2f_1$, $f_3 = 3f_1$, ...

**Pipe open at both ends:**
$$L = n\frac{\lambda_n}{2}, \quad f_n = \frac{nv}{2L}$$

**Pipe closed at one end:**
$$L = (2n-1)\frac{\lambda_n}{4}, \quad f_n = \frac{(2n-1)v}{4L}$$

Only odd harmonics ($f_1, 3f_1, 5f_1, ...$).

### 3.6 Resonance

A system resonates when driven at its **natural frequency**, absorbing maximum energy. In strings and air columns, resonance produces standing waves with large amplitude — the basis of musical instruments.

### 3.7 Beats

When two waves of slightly different frequencies $f_1$ and $f_2$ interfere, the amplitude modulates at the **beat frequency**:

$$f_{beat} = |f_1 - f_2|$$

Beats are used to tune instruments: when beat frequency approaches zero, the frequencies match.

### 3.8 Reflection and Refraction

- **Reflection:** wave bounces off a boundary. At a fixed end, the reflected wave is inverted ($\pi$ phase shift); at a free end, it is not inverted.
- **Refraction:** wave changes speed (and direction) when entering a new medium.

---

## 4 | Common Problem Types

### Type 1: Wave speed from frequency and wavelength
> A wave has $f = 50\ \text{Hz}$, $\lambda = 6\ \text{m}$. Find speed.

**Solution:**
$$v = f\lambda = 50 \times 6 = 300\ \text{m/s}$$

### Type 2: Standing wave on a string
> A $1\ \text{m}$ string fixed at both ends has wave speed $300\ \text{m/s}$. Find the fundamental and second harmonic frequencies.

**Solution:**
$$f_1 = \frac{v}{2L} = \frac{300}{2 \times 1} = 150\ \text{Hz}$$
$$f_2 = 2f_1 = 300\ \text{Hz}$$

### Type 3: Closed pipe resonance
> A closed pipe has fundamental $f_1 = 200\ \text{Hz}$, $v = 340\ \text{m/s}$. Find pipe length.

**Solution:**
$$f_1 = \frac{v}{4L} \Rightarrow L = \frac{v}{4f_1} = \frac{340}{4 \times 200} = 0.425\ \text{m}$$

### Type 4: Beat frequency
> Two tuning forks at $440\ \text{Hz}$ and $443\ \text{Hz}$ sound together. Find the beat frequency.

**Solution:**
$$f_{beat} = |f_1 - f_2| = |440 - 443| = 3\ \text{Hz}$$

### Type 5: Travelling wave equation
> A wave has $A = 0.02\ \text{m}$, $f = 10\ \text{Hz}$, $v = 5\ \text{m/s}$, starting at equilibrium. Write $y(x,t)$.

**Solution:**
$$\lambda = \frac{v}{f} = 0.5\ \text{m}, \quad k = \frac{2\pi}{\lambda} = 4\pi, \quad \omega = 2\pi f = 20\pi$$
$$y(x,t) = 0.02\sin(4\pi x - 20\pi t)\ \text{m}$$

---

## 5 | Cross-Links

- [[07_Oscillations]] — waves are propagating oscillations; SHM describes each particle
- [[04_Work_Energy_and_Power]] — waves transport energy
- [[05_Momentum]] — wave momentum in radiation pressure
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — sinusoidal functions, trigonometry
