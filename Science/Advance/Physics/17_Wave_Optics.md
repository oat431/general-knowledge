---
tags:
  - physics
  - advance
  - wave-optics
  - interference
  - diffraction
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Wave Optics — ทัศนพจน์คลื่น

> *"Light is a wave that shows us the world, and interference is the signature of its wave nature."* — Thomas Young

Wave optics (physical optics) reveals the wave nature of light through phenomena that geometric (ray) optics cannot explain. Interference, diffraction, and polarization demonstrate that light behaves as a wave with amplitude and phase. Young's double-slit experiment provides the definitive evidence that light interferes with itself, producing bright and dark fringes. Diffraction patterns from single slits and gratings encode information about wavelength. Thin film interference creates the iridescent colors seen in soap bubbles and oil slicks.

In ว302, this is the capstone of the optics sequence. Students move from the ray model (geometric optics) to the wave model, applying principles of superposition and path differences to predict interference and diffraction patterns. The resolution limit of optical instruments (telescopes, microscopes) connects wave optics to the practical limits of observation, linking physics to astronomy and biology.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Electromagnetism foundations) | — |
| **Semester 2** | Interference (double-slit), diffraction (single-slit, grating), polarization, thin films, resolution | Calculate fringe spacing; diffraction minima; grating equation; thin film conditions; Rayleigh criterion |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ทัศนพจน์คลื่น | Wave optics (physical optics) | Wave nature of light |
| การแทรกสอด | Interference | Superposition |
| การเลี้ยวเบน | Diffraction | Bending around obstacles |
| ประสาน | Coherence | Constant phase |
| ความยาวทางเดิน | Path difference | $\Delta = d\sin\theta$ |
| ทดลองสองช่องของยัง | Young's double-slit | $\Delta y = \frac{\lambda L}{d}$ |
| การเลี้ยวเบนช่องเดียว | Single-slit diffraction | $a\sin\theta = m\lambda$ |
| เกรตติ้งเลี้ยวเบน | Diffraction grating | $d\sin\theta = m\lambda$ |
| ฟิล์มบาง | Thin film | $2nt = m\lambda$ |
| โพลาไรเซชัน | Polarization | Transverse wave |
| เกณฑ์เรย์ลี | Rayleigh criterion | Resolution limit |
| แถบสว่าง/มืด | Bright/dark fringe | Max/min intensity |

---

## 3 | Key Concepts

### 3.1 Young's Double-Slit Experiment

Two coherent slits separated by $d$ produce interference fringes on a screen at distance $L$.

**Bright fringes (constructive):** $d\sin\theta = m\lambda$, $m = 0, 1, 2, \ldots$

**Dark fringes (destructive):** $d\sin\theta = (m + \frac{1}{2})\lambda$

For small angles ($\sin\theta \approx \tan\theta$), fringe spacing:

$$\Delta y = \frac{\lambda L}{d}$$

### 3.2 Single-Slit Diffraction

Light through a narrow slit spreads out and interferes with itself.

**Minima (dark):** $a\sin\theta = m\lambda$, $m = 1, 2, 3, \ldots$

Where $a$ is slit width. Central maximum width: $\Delta y = \frac{2\lambda L}{a}$.

### 3.3 Diffraction Grating

Multiple parallel slits produce sharp, bright maxima:

$$d\sin\theta = m\lambda, \quad m = 0, 1, 2, \ldots$$

Where $d$ is grating spacing. More slits → sharper, brighter maxima. Gratings are used in spectroscopy to separate wavelengths.

### 3.4 Thin Film Interference

Light reflected from the top and bottom of a thin film of thickness $t$ and index $n$ interferes.

**With phase reversal (one reflection):**

Constructive: $2nt = (m + \frac{1}{2})\lambda$

Destructive: $2nt = m\lambda$

**Without phase reversal (both or neither):**

Constructive: $2nt = m\lambda$

Destructive: $2nt = (m + \frac{1}{2})\lambda$

The $\lambda$ here is the wavelength **in vacuum**. The effective wavelength in the film is $\lambda_n = \lambda/n$.

### 3.5 Polarization

EM waves are transverse, so they can be polarized. Methods:

- **Polarizers:** Selective absorption (Malus's law: $I = I_0\cos^2\theta$)
- **Reflection:** Brewster's angle: $\tan\theta_B = n_2/n_1$
- **Scattering:** Sky polarization

### 3.6 Resolution and Rayleigh Criterion

Two point sources are just resolvable when the center of one diffraction pattern falls on the first minimum of the other:

$$\theta_{\min} = 1.22\frac{\lambda}{D}$$

Where $D$ is the aperture diameter. This limits telescope and microscope resolution — larger apertures resolve finer details.

---

## 4 | Common Problem Types

### Type 1: Double-Slit Fringe Spacing
> Slits are 0.2 mm apart, screen is 2 m away, $\lambda = 600$ nm. Find fringe spacing.

**Solution:**

$$\Delta y = \frac{\lambda L}{d} = \frac{(600 \times 10^{-9})(2)}{0.2 \times 10^{-3}} = 6 \times 10^{-3} \text{ m} = 6 \text{ mm}$$

### Type 2: Single-Slit First Minimum
> A slit of width 0.1 mm is illuminated by 500 nm light. Find the first dark fringe angle.

**Solution:**

$$a\sin\theta = \lambda, \quad \sin\theta = \frac{500 \times 10^{-9}}{0.1 \times 10^{-3}} = 5 \times 10^{-3}$$

$$\theta \approx 0.286° \text{ (small angle)}$$

### Type 3: Diffraction Grating
> A grating has 5000 lines/cm. Find the angle for the 2nd order maximum at 500 nm.

**Solution:**

$$d = \frac{1}{5000} \text{ cm} = 2 \times 10^{-6} \text{ m}$$

$$\sin\theta = \frac{m\lambda}{d} = \frac{2 \times 500 \times 10^{-9}}{2 \times 10^{-6}} = 0.5$$

$$\theta = 30°$$

### Type 4: Thin Film (Anti-Reflective Coating)
> A film ($n = 1.38$) of thickness 100 nm is on glass ($n = 1.5$). Find $\lambda$ for destructive interference (normal incidence).

**Solution:** Both reflections have phase reversal (air-film and film-glass both go from low to high $n$), so for destructive:

$$2nt = (m + \tfrac{1}{2})\lambda, \quad m = 0: \quad \lambda = 2nt = 2(1.38)(100) = 276 \text{ nm}$$

This is UV — a real anti-reflective coating is designed for visible $\lambda$ by choosing appropriate $t$.

### Type 5: Rayleigh Criterion
> A telescope has aperture $D = 0.1$ m. Find the minimum angular separation at $\lambda = 550$ nm.

**Solution:**

$$\theta_{\min} = 1.22\frac{\lambda}{D} = 1.22\frac{550 \times 10^{-9}}{0.1} = 6.71 \times 10^{-6} \text{ rad} \approx 1.38 \text{ arcsec}$$

---

## 5 | Cross-Links

- [[16_Light_and_Optics]] — Wave optics extends geometric (ray) optics
- [[15_Electromagnetic_Waves]] — Interference and diffraction are EM wave phenomena
- [[09_Sound]] — Sound also exhibits interference and diffraction
- [[Fundamental/08_Waves]] — Superposition principle underlies all interference
