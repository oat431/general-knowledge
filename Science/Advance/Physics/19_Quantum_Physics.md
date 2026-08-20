---
tags:
  - physics
  - advance
  - quantum-physics
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว303"]
---

# Quantum Physics — ฟิสิกส์ควอนตัม

> *"If you think you understand quantum mechanics, you don't understand quantum mechanics."* — Richard Feynman

Quantum physics emerged at the dawn of the 20th century when classical physics could not explain blackbody radiation, the photoelectric effect, and atomic spectra. Planck's quantum hypothesis (1900) and Einstein's photon theory (1905) introduced the radical idea that energy is quantized — it comes in discrete packets called quanta. This wave-particle duality of light and matter fundamentally changed our view of reality and led to technologies from lasers to transistors to quantum computing.

For the ว303 curriculum, students study the photoelectric effect, wave-particle duality (de Broglie wavelength), the uncertainty principle, and Compton scattering. These topics form the conceptual bridge between classical physics and the modern quantum description of atoms, nuclei, and elementary particles.

---

## 1 | Course Coverage

### ม.6 (ว303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Blackbody radiation (Planck), photoelectric effect, photon energy E=hf, wave-particle duality, de Broglie wavelength | Compute photon energy and momentum; solve photoelectric problems (work function, stopping potential, kinetic energy); calculate de Broglie wavelengths |
| **Semester 2** | Uncertainty principle, Compton scattering, double-slit experiment with particles | Apply Heisenberg uncertainty relation; compute Compton wavelength shift; interpret wave-particle duality in experiments |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ควอนตัม | Quantum | Discrete unit of a physical quantity |
| สมการของพลังค์ | Planck's equation | $E = hf$ |
| ค่าคงที่ของพลังค์ | Planck's constant | $h = 6.626 \times 10^{-34}$ J·s |
| ปรากฏการณ์โฟโตอิเล็กทริก | Photoelectric effect | Emission of electrons from metal by light |
| งานฟังก์ชัน | Work function | $W$ or $\phi$, minimum energy to eject electron |
| ศักย์ไฟฟ้าหยุด | Stopping potential | $V_s$, voltage to stop fastest electron |
| ความยาวคลื่นเดอบรอย | de Broglie wavelength | $\lambda = h/p$ |
| ทวิตาภาคของคลื่น-อนุภาค | Wave-particle duality | Light and matter show both natures |
| หลักความไม่แน่นอน | Uncertainty principle | $\Delta x \, \Delta p \geq \hbar/2$ |
| กระจายคอมปตัน | Compton scattering | Photon scatters off free electron |
| ความยาวคลื่นคอมปตัน | Compton wavelength | $\lambda_C = h/(m_e c) = 2.43 \times 10^{-12}$ m |
| ความถี่เกิดขอ้บ | Threshold frequency | $f_0 = W/h$ |
| โฟตอน | Photon | Quantum of light, energy $E = hf$ |

---

## 3 | Key Concepts

### 3.1 Planck's Quantum Hypothesis

Max Planck (1900) proposed that blackbody radiation is emitted in discrete energy packets:

$$E = hf = \frac{hc}{\lambda}$$

where $h = 6.626 \times 10^{-34}$ J·s is Planck's constant and $f$ is the frequency. This resolved the "ultraviolet catastrophe" of classical physics.

### 3.2 The Photoelectric Effect

When light shines on a metal surface, electrons are ejected **only if** the photon energy exceeds the metal's **work function** $W$ (งานฟังก์ชัน). Key observations that classical wave theory could not explain:

- No emission below threshold frequency $f_0 = W/h$, regardless of intensity.
- Emission is instantaneous (no delay), even at low intensity.
- Maximum kinetic energy depends on frequency, not intensity.

Einstein's explanation: each photon of energy $hf$ transfers its energy to a single electron. The **photoelectric equation** is:

$$K_{\max} = hf - W$$

where $K_{\max}$ is the maximum kinetic energy of ejected electrons and $W$ is the work function.

The **stopping potential** $V_s$ relates to kinetic energy:

$$K_{\max} = e V_s$$

### 3.3 Wave-Particle Duality

Light exhibits wave behavior (interference, diffraction) and particle behavior (photoelectric effect, Compton scattering). Louis de Broglie (1924) proposed that **matter** also has wave properties. The **de Broglie wavelength** of a particle with momentum $p$ is:

$$\lambda = \frac{h}{p} = \frac{h}{mv}$$

For macroscopic objects this wavelength is vanishingly small, which is why wave behavior is not observed in everyday life. For electrons and other subatomic particles, $\lambda$ is comparable to atomic scales.

### 3.4 The Uncertainty Principle

Werner Heisenberg (1927) showed that certain pairs of physical properties cannot be simultaneously known to arbitrary precision. The most famous form:

$$\Delta x \cdot \Delta p \geq \frac{\hbar}{2}$$

where $\hbar = h/(2\pi) = 1.055 \times 10^{-34}$ J·s. A second form relates energy and time:

$$\Delta E \cdot \Delta t \geq \frac{\hbar}{2}$$

This is not a measurement limitation but a fundamental property of nature — a particle does not simultaneously have a precise position and momentum.

### 3.5 Compton Scattering

Arthur Compton (1923) observed that X-rays scattered by free electrons undergo a **wavelength shift** that depends on the scattering angle. Treating the photon as a particle with energy $E = hf$ and momentum $p = h/\lambda$, and applying relativistic energy-momentum conservation gives:

$$\Delta \lambda = \lambda' - \lambda = \frac{h}{m_e c}(1 - \cos\theta) = \lambda_C(1 - \cos\theta)$$

where $\lambda_C = h/(m_e c) = 2.43 \times 10^{-12}$ m is the **Compton wavelength** of the electron, and $\theta$ is the scattering angle of the photon. At $\theta = 0$ there is no shift; at $\theta = 180°$ the shift is maximum at $2\lambda_C$.

This experiment provided strong evidence for the particle nature of light.

### 3.6 Photon Momentum

Although massless, a photon carries momentum:

$$p = \frac{E}{c} = \frac{hf}{c} = \frac{h}{\lambda}$$

---

## 4 | Common Problem Types

### Type 1: Photoelectric effect
> Light of wavelength 250 nm strikes a sodium surface with work function 2.28 eV. Find the maximum kinetic energy and stopping potential.

**Solution:**

Step 1 — Photon energy:

$$E = \frac{hc}{\lambda} = \frac{(6.626 \times 10^{-34})(3 \times 10^8)}{250 \times 10^{-9}} = 7.95 \times 10^{-19} \ \text{J} = 4.96 \ \text{eV}$$

Step 2 — Maximum kinetic energy:

$$K_{\max} = hf - W = 4.96 - 2.28 = 2.68 \ \text{eV}$$

Step 3 — Stopping potential:

$$V_s = \frac{K_{\max}}{e} = 2.68 \ \text{V}$$

---

### Type 2: de Broglie wavelength
> Find the de Broglie wavelength of an electron accelerated through 100 V.

**Solution:**

Kinetic energy: $K = eV = 100$ eV $= 1.60 \times 10^{-17}$ J

For non-relativistic electrons: $K = \frac{p^2}{2m_e}$, so $p = \sqrt{2m_e K}$

$$p = \sqrt{2(9.11 \times 10^{-31})(1.60 \times 10^{-17})} = 5.40 \times 10^{-24} \ \text{kg·m/s}$$

$$\lambda = \frac{h}{p} = \frac{6.626 \times 10^{-34}}{5.40 \times 10^{-24}} \approx 1.23 \times 10^{-10} \ \text{m} = 0.123 \ \text{nm}$$

**Shortcut:** $\lambda (\text{nm}) \approx \frac{1.226}{\sqrt{V(\text{volts})}}$, giving $\lambda \approx 0.123$ nm. ✓

---

### Type 3: Compton scattering
> An X-ray photon of wavelength 0.050 nm scatters at 60° from a free electron. Find the scattered photon's wavelength and the electron's kinetic energy.

**Solution:**

$$\Delta\lambda = \lambda_C(1 - \cos 60°) = (2.43 \times 10^{-12})(1 - 0.5) = 1.215 \times 10^{-12} \ \text{m}$$

$$\lambda' = 0.050 + 0.00122 \approx 0.05122 \ \text{nm}$$

The electron's kinetic energy equals the photon's energy loss:

$$K_e = hc\left(\frac{1}{\lambda} - \frac{1}{\lambda'}\right) = (6.626 \times 10^{-34})(3 \times 10^8)\left(\frac{1}{5.0 \times 10^{-11}} - \frac{1}{5.122 \times 10^{-11}}\right)$$

$$K_e \approx 2.84 \times 10^{-16} \ \text{J} \approx 1.77 \ \text{keV}$$

---

### Type 4: Uncertainty principle
> An electron is confined to a region of 0.10 nm (atomic scale). Estimate the minimum uncertainty in its momentum.

**Solution:**

$$\Delta p \geq \frac{\hbar}{2\Delta x} = \frac{1.055 \times 10^{-34}}{2 \times 1.0 \times 10^{-10}} \approx 5.28 \times 10^{-25} \ \text{kg·m/s}$$

This corresponds to a speed of roughly $5.8 \times 10^5$ m/s — significant at atomic scales, which explains why electrons cannot be localized within a nucleus.

---

## 5 | Cross-Links

- [[18_Special_Relativity]] — Photon energy-momentum uses relativistic relations
- [[20_Atomic_Physics]] — Bohr model and quantized energy levels build on quantum ideas
- [[15_Electromagnetic_Waves]] — Light as wave; photon theory adds particle nature
- [[22_Particle_Physics]] — Quantum field theory extends quantum physics to all particles
