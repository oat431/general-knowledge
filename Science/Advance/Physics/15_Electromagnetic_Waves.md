---
tags:
  - physics
  - advance
  - electromagnetic-waves
  - em-spectrum
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Electromagnetic Waves — คลื่นแม่เหล็กไฟฟ้า

> *"The discovery of electromagnetic waves was the greatest intellectual triumph of the nineteenth century."* — Heinrich Hertz

Electromagnetic (EM) waves are self-propagating oscillations of electric and magnetic fields that travel through space at the speed of light. Unlike mechanical waves, they require no medium and can traverse a vacuum. Maxwell's equations unify electricity, magnetism, and optics into a single framework, predicting that light is an electromagnetic wave. The EM spectrum spans from low-frequency radio waves to high-frequency gamma rays, each region with distinct applications from communication to medical imaging.

In ว302, students learn that EM waves are the natural consequence of accelerating charges. The concepts of wavelength, frequency, and speed apply universally across the spectrum. This topic bridges the gap between the circuit-level electromagnetism of earlier chapters and the wave optics of the following chapters, establishing that visible light is simply a narrow band of the broader EM spectrum.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Electrostatics, circuits, magnetism foundations) | — |
| **Semester 2** | EM spectrum, wave properties, Maxwell's equations (conceptual), light as EM wave | Identify EM spectrum regions; relate $v = f\lambda$; understand EM wave nature |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| คลื่นแม่เหล็กไฟฟ้า | Electromagnetic wave | Transverse, no medium |
| สมการของแมกซ์เวลล์ | Maxwell's equations | Four fundamental equations |
| ความเร็วแสง | Speed of light | $c = 3 \times 10^8$ m/s |
| สเปกตรัมแม่เหล็กไฟฟ้า | EM spectrum | Radio → Gamma |
| คลื่นวิทยุ | Radio wave | $f < 10^9$ Hz |
| ไมโครเวฟ | Microwave | Cooking, radar |
| อินฟราเรด | Infrared (IR) | Heat radiation |
| แสงที่มองเห็น | Visible light | 400–700 nm |
| อัลตราไวโอเลต | Ultraviolet (UV) | Sunburn, sterilization |
| รังสีเอกซ์ | X-ray | Medical imaging |
| รังสีแกมมา | Gamma ray | Nuclear, highest energy |
| โพลาไรเซชัน | Polarization | $\perp$ to propagation |

---

## 3 | Key Concepts

### 3.1 Maxwell's Equations (Conceptual)

Maxwell's four equations summarize electromagnetism:

1. **Gauss's law (electric):** Electric charges produce electric fields.
$$\oint \vec{E}\cdot d\vec{A} = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

2. **Gauss's law (magnetic):** No magnetic monopoles exist.
$$\oint \vec{B}\cdot d\vec{A} = 0$$

3. **Faraday's law:** Changing magnetic fields produce electric fields.
$$\oint \vec{E}\cdot d\vec{l} = -\frac{d\Phi_B}{dt}$$

4. **Ampère-Maxwell law:** Currents and changing electric fields produce magnetic fields.
$$\oint \vec{B}\cdot d\vec{l} = \mu_0 I + \mu_0\varepsilon_0\frac{d\Phi_E}{dt}$$

### 3.2 EM Wave Properties

EM waves are transverse: $\vec{E} \perp \vec{B} \perp$ direction of propagation. In vacuum:

$$c = \frac{1}{\sqrt{\mu_0\varepsilon_0}} = 3 \times 10^8 \text{ m/s}$$

Wave relationship: $c = f\lambda$. In a medium with index $n$:

$$v = \frac{c}{n}, \quad n = \frac{c}{v}$$

### 3.3 Energy and Intensity

Energy density: $u = \frac{1}{2}\varepsilon_0 E^2 + \frac{B^2}{2\mu_0}$ (equal contributions).

For an EM wave: $u = \varepsilon_0 E^2 = \frac{B^2}{\mu_0}$, and $E = cB$.

Intensity (average power per area): $I = \frac{E_0^2}{2\mu_0 c}$ where $E_0$ is the peak electric field.

### 3.4 The EM Spectrum

| Region | Wavelength | Frequency | Applications |
|---|---|---|---|
| Radio | $>1$ m | $<300$ MHz | Broadcasting, TV |
| Microwave | 1 mm – 1 m | 300 MHz – 300 GHz | Cooking, radar, WiFi |
| Infrared | 700 nm – 1 mm | $10^{12}$–$10^{14}$ Hz | Heat, remote controls |
| Visible | 400–700 nm | $4.3$–$7.5 \times 10^{14}$ Hz | Human vision |
| Ultraviolet | 10–400 nm | $10^{15}$–$10^{16}$ Hz | Sterilization, fluorescence |
| X-ray | 0.01–10 nm | $10^{16}$–$10^{19}$ Hz | Medical, crystallography |
| Gamma | $<0.01$ nm | $>10^{19}$ Hz | Cancer treatment, nuclear |

### 3.5 Polarization

EM waves can be polarized — the electric field oscillates in a preferred direction. Unpolarized light has random orientations. A polarizer transmits only the component aligned with its axis:

$$I = I_0 \cos^2\theta \quad \text{(Malus's law)}$$

Polarization demonstrates the transverse nature of EM waves.

---

## 4 | Common Problem Types

### Type 1: Wavelength-Frequency Relation
> A radio station broadcasts at 100 MHz. Find the wavelength.

**Solution:**

$$\lambda = \frac{c}{f} = \frac{3 \times 10^8}{100 \times 10^6} = 3 \text{ m}$$

### Type 2: Speed in a Medium
> Light travels through glass with $n = 1.5$. Find its speed.

**Solution:**

$$v = \frac{c}{n} = \frac{3 \times 10^8}{1.5} = 2 \times 10^8 \text{ m/s}$$

### Type 3: Malus's Law
> Polarized light with intensity $I_0$ passes through a polarizer at 30° to the polarization axis. Find the transmitted intensity.

**Solution:**

$$I = I_0 \cos^2(30°) = I_0 \times (0.866)^2 = 0.75\, I_0$$

### Type 4: Energy of a Photon
> Find the energy of a visible light photon with $\lambda = 500$ nm.

**Solution:**

$$E = hf = \frac{hc}{\lambda} = \frac{(6.626 \times 10^{-34})(3 \times 10^8)}{500 \times 10^{-9}} = 3.97 \times 10^{-19} \text{ J} \approx 2.48 \text{ eV}$$

---

## 5 | Cross-Links

- [[09_Sound]] — Contrast mechanical waves (need medium) with EM waves (no medium)
- [[13_Magnetism]] — Accelerating charges produce EM waves
- [[14_Electromagnetic_Induction]] — Faraday's law is part of Maxwell's equations
- [[16_Light_and_Optics]] — Visible light is one region of the EM spectrum
- [[17_Wave_Optics]] — Interference and diffraction of EM waves
