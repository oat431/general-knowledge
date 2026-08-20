---
tags:
  - physics
  - advance
  - atomic-physics
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว303"]
---

# Atomic Physics — ฟิสิกส์ปรมาณู

> *"All matter originates and exists only by virtue of a force which brings the particle of an atom to vibration and holds this most minute solar system of the atom together."* — Max Planck

Atomic physics studies the structure and behavior of atoms, focusing on the arrangement of electrons around the nucleus and the interaction of atoms with light. The Bohr model (1913) provided the first successful quantum description of the hydrogen atom, explaining its discrete emission spectrum. While later superseded by full quantum mechanics, the Bohr model remains an essential pedagogical tool and a stepping stone to understanding atomic structure, quantum numbers, and electron configurations.

In the ว303 curriculum, students learn the Bohr model, hydrogen energy levels, emission and absorption spectra, an introduction to quantum numbers, and the principles of electron configuration that explain the periodic table's structure.

---

## 1 | Course Coverage

### ม.6 (ว303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Bohr model of hydrogen, energy levels, emission and absorption spectra, spectral series | Calculate energy levels and transition wavelengths; identify spectral series (Lyman, Balmer, Paschen); distinguish emission vs absorption spectra |
| **Semester 2** | Quantum numbers (n, l, m_l, m_s), Pauli exclusion principle, electron configuration, periodic table connection | Write electron configurations; apply Pauli principle and Hund's rule; explain periodic trends |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| โมเดลของบัวร์ | Bohr model | Quantized circular orbits for hydrogen |
| ระดับพลังงาน | Energy level | Discrete allowed energies $E_n$ |
| สถานะพื้น | Ground state | Lowest energy state, $n = 1$ |
| สถานะกระตุ้น | Excited state | $n > 1$ |
| สเปกตรัมการปล่อยกลาย | Emission spectrum | Light emitted when electron drops to lower level |
| สเปกตรัมการดูดกลืน | Absorption spectrum | Dark lines from absorbed photons |
| ชุดสเปกตรัม | Spectral series | Lyman (UV), Balmer (visible), Paschen (IR) |
| เลขควอนตัมหลัก | Principal quantum number | $n = 1, 2, 3, \ldots$ |
| เลขควอนตัมโมเมนตัมเชิงมุม | Azimuthal quantum number | $l = 0, 1, \ldots, n-1$ |
| เลขควอนตัมแม่เหล็ก | Magnetic quantum number | $m_l = -l, \ldots, +l$ |
| เลขควอนตัมสปิน | Spin quantum number | $m_s = \pm 1/2$ |
| หลักกีดกันของเพาลี | Pauli exclusion principle | No two electrons share all four quantum numbers |
| การจัดเรียงอิเล็กตรอน | Electron configuration | Distribution of electrons in orbitals |
| กฎของฮุนด์ | Hund's rule | Fill degenerate orbitals singly first |
| ค่าคงที่ริดเบิร์ก | Rydberg constant | $R = 1.097 \times 10^7$ m⁻¹ |

---

## 3 | Key Concepts

### 3.1 The Bohr Model

Niels Bohr (1913) proposed a model of the hydrogen atom based on three postulates:

1. Electrons orbit the nucleus in **circular orbits** of specific radii (quantized angular momentum).
2. Electrons do not radiate energy while in these **stationary orbits**.
3. Energy is emitted or absorbed **only** when an electron transitions between orbits, as a photon of energy $hf = |E_i - E_f|$.

The quantization condition for angular momentum:

$$L = m_e v r = n\hbar, \quad n = 1, 2, 3, \ldots$$

### 3.2 Bohr Radius and Orbital Radius

The radius of the $n$-th orbit:

$$r_n = n^2 \left(\frac{\hbar^2}{m_e k e^2}\right) = n^2 \, a_0$$

where $a_0 = 0.0529$ nm is the **Bohr radius** (รัศมีบัวร์), the radius of the ground state orbit.

### 3.3 Energy Levels of Hydrogen

The total energy of the $n$-th state of hydrogen:

$$E_n = -\frac{13.6 \ \text{eV}}{n^2}$$

- $E_1 = -13.6$ eV (ground state)
- $E_2 = -3.40$ eV (first excited state)
- $E_\infty = 0$ (ionization)

The **ionization energy** of hydrogen (energy to remove the electron from ground state) is 13.6 eV.

### 3.4 Spectral Series

When an electron transitions from a higher level $n_i$ to a lower level $n_f$, a photon is emitted with wavelength given by the **Rydberg formula**:

$$\frac{1}{\lambda} = R\left(\frac{1}{n_f^2} - \frac{1}{n_i^2}\right)$$

where $R = 1.097 \times 10^7$ m⁻¹ is the Rydberg constant.

| Series | $n_f$ | Region | Notes |
|---|---|---|---|
| Lyman | 1 | Ultraviolet | Transitions to ground state |
| Balmer | 2 | Visible | Includes Hα (656 nm, red) |
| Paschen | 3 | Infrared | First infrared series |
| Brackett | 4 | Far infrared | — |
| Pfund | 5 | Far infrared | — |

### 3.5 Emission vs Absorption Spectra

- **Emission spectrum (สเปกตรัมการปล่อยออก):** A hot, low-pressure gas emits photons at specific wavelengths — bright lines on a dark background.
- **Absorption spectrum (สเปกตรัมการดูดกลืน):** A continuous spectrum passes through a cool gas, which absorbs photons at specific wavelengths — dark lines on a bright background.

The absorption lines occur at exactly the same wavelengths as the emission lines for the same element, because the same energy-level transitions are involved.

### 3.6 Quantum Numbers

Full quantum mechanics describes atomic states with four quantum numbers:

| Number | Symbol | Allowed values | Description |
|---|---|---|---|
| Principal | $n$ | $1, 2, 3, \ldots$ | Energy level / shell |
| Azimuthal | $l$ | $0, 1, \ldots, n-1$ | Orbital shape (s, p, d, f) |
| Magnetic | $m_l$ | $-l, \ldots, +l$ | Orientation in space |
| Spin | $m_s$ | $+\frac{1}{2}, -\frac{1}{2}$ | Electron spin direction |

The subshell letters: $l=0 \to s$, $l=1 \to p$, $l=2 \to d$, $l=3 \to f$.

### 3.7 Pauli Exclusion Principle and Electron Configuration

The **Pauli exclusion principle** (หลักกีดกันของเพาลี) states that no two electrons in an atom can have the same set of all four quantum numbers. This means each orbital can hold at most **2 electrons** (with opposite spins).

The capacity of each subshell:
- $s$: 2 electrons (1 orbital)
- $p$: 6 electrons (3 orbitals)
- $d$: 10 electrons (5 orbitals)
- $f$: 14 electrons (7 orbitals)

**Hund's rule** (กฎของฮุนด์): electrons fill degenerate orbitals (same $n$ and $l$) singly with parallel spins before pairing up.

---

## 4 | Common Problem Types

### Type 1: Hydrogen energy levels and transitions
> Find the wavelength of the photon emitted when an electron in hydrogen transitions from $n = 4$ to $n = 2$ (Balmer series).

**Solution:**

$$\frac{1}{\lambda} = R\left(\frac{1}{n_f^2} - \frac{1}{n_i^2}\right) = 1.097 \times 10^7\left(\frac{1}{4} - \frac{1}{16}\right)$$

$$\frac{1}{\lambda} = 1.097 \times 10^7 \times \frac{3}{16} = 2.057 \times 10^6 \ \text{m}^{-1}$$

$$\lambda = 4.86 \times 10^{-7} \ \text{m} = 486 \ \text{nm}$$

This is the Hβ line (blue-green) in the visible Balmer series. ✓

---

### Type 2: Ionization energy
> What is the minimum frequency of light needed to ionize hydrogen from its ground state?

**Solution:**

$$E_{\text{ionize}} = 13.6 \ \text{eV} = 2.18 \times 10^{-18} \ \text{J}$$

$$f = \frac{E}{h} = \frac{2.18 \times 10^{-18}}{6.626 \times 10^{-34}} \approx 3.29 \times 10^{15} \ \text{Hz}$$

This is in the ultraviolet (Lyman limit). ✓

---

### Type 3: Electron configuration
> Write the electron configuration of iron (Fe, Z = 26).

**Solution:**

Following the Aufbau principle (fill lowest energy first):

$$1s^2 \, 2s^2 \, 2p^6 \, 3s^2 \, 3p^6 \, 4s^2 \, 3d^6$$

Note: the 4s orbital fills before 3d. Fe has 6 electrons in the 3d subshell. The two 4s electrons and the partially filled 3d subshell give iron its characteristic chemical and magnetic properties. ✓

---

### Type 4: Orbital velocity in Bohr model
> Find the speed of the electron in the ground state of hydrogen.

**Solution:**

From $L = m_e v r = \hbar$ and $r_1 = a_0 = 5.29 \times 10^{-11}$ m:

$$v_1 = \frac{\hbar}{m_e a_0} = \frac{1.055 \times 10^{-34}}{(9.11 \times 10^{-31})(5.29 \times 10^{-11})} \approx 2.19 \times 10^6 \ \text{m/s}$$

This is about $\alpha c \approx c/137$, where $\alpha \approx 1/137$ is the fine-structure constant. ✓

---

## 5 | Cross-Links

- [[19_Quantum_Physics]] — Quantization of energy is the foundation of atomic models
- [[18_Special_Relativity]] — Fine structure corrections require relativistic treatment
- [[21_Nuclear_Physics]] — The nucleus inside the atom; nuclear properties affect atomic spectra
- [[15_Electromagnetic_Waves]] — Spectra are analyzed using EM wave properties
