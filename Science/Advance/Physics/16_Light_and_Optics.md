---
tags:
  - physics
  - advance
  - optics
  - light
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Light and Optics — แสงและทัศนศาสตร์

> *"Optics is the study of light, the swiftest messenger we know."* — David Brewster

Optics is the study of light and its interactions with matter. Geometric (ray) optics treats light as straight-line rays that reflect off surfaces and refract at boundaries. The laws of reflection and refraction (Snell's law) govern mirrors and lenses, forming the basis of optical instruments from eyeglasses to telescopes. Total internal reflection enables fiber optic communication. This chapter builds on the EM wave nature of light established previously, while focusing on the practical ray-based analysis appropriate for most everyday optical phenomena.

In ว302, students learn to trace light rays through optical systems, apply the thin lens and mirror equations, and understand image formation. The transition from geometric optics to wave optics (interference, diffraction) follows in the next chapter, completing the picture of light's dual wave-particle nature.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | (Electromagnetism foundations) | — |
| **Semester 2** | Reflection, refraction, Snell's law, lenses, mirrors, optical instruments, TIR | Ray tracing; thin lens/mirror equations; magnification; optical instruments |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| แสง | Light | EM wave, $v = c/n$ |
| การสะท้อน | Reflection | $\theta_i = \theta_r$ |
| การหักเห | Refraction | Snell's law |
| กฎของสแนลล์ | Snell's law | $n_1\sin\theta_1 = n_2\sin\theta_2$ |
| ดัชนีหักเห | Refractive index | $n = c/v$ |
| การสะท้อนกลับทั้งหมด | Total internal reflection | $\theta > \theta_c$ |
| มุมวิกฤต | Critical angle | $\sin\theta_c = n_2/n_1$ |
| เลนส์ | Lens | Converging (+) / Diverging (−) |
| กระจก | Mirror | Concave / Convex |
| ระยะโฟกัส | Focal length | $f$ (m) |
| การขยาย | Magnification | $M = -d_i/d_o = h_i/h_o$ |
| ภาพจริง | Real image | Formed by actual rays |
| ภาพซ้อน | Virtual image | Apparent, cannot project |
| กล้องกำลังแสง | Telescope | Angular magnification |
| กล้องจุลทรรศน์ | Microscope | Compound magnification |

---

## 3 | Key Concepts

### 3.1 Reflection

Law of reflection: angle of incidence = angle of reflection (both measured from the normal).

$$\theta_i = \theta_r$$

### 3.2 Refraction and Snell's Law

$$n_1 \sin\theta_1 = n_2 \sin\theta_2$$

Where $n$ is the refractive index. Light bends toward the normal when entering a denser medium ($n_2 > n_1$).

### 3.3 Total Internal Reflection

When light travels from a denser to a less dense medium ($n_1 > n_2$), beyond the critical angle all light is reflected:

$$\sin\theta_c = \frac{n_2}{n_1} \quad (n_1 > n_2)$$

This principle enables fiber optics, prisms in binoculars, and the brilliance of diamonds ($n \approx 2.42$).

### 3.4 Mirrors

**Mirror equation:**

$$\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$$

Sign convention: $d_o > 0$ for real objects; $d_i > 0$ for real images (concave, $d_o > f$); $f > 0$ for concave, $f < 0$ for convex.

**Magnification:** $M = -\frac{d_i}{d_o}$

- Concave mirror: converging; can form real or virtual images
- Convex mirror: diverging; always virtual, diminished, upright

### 3.5 Thin Lenses

**Lens equation (same form as mirror):**

$$\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$$

Sign convention: $f > 0$ for converging (convex) lenses; $f < 0$ for diverging (concave) lenses.

**Magnification:** $M = -\frac{d_i}{d_o}$

**Lens maker's equation:**

$$\frac{1}{f} = (n - 1)\left(\frac{1}{R_1} - \frac{1}{R_2}\right)$$

### 3.6 Optical Instruments

**Magnifying glass (simple magnifier):** $M = \frac{25\text{ cm}}{f}$ (near point 25 cm)

**Compound microscope:** $M = M_{\text{objective}} \times M_{\text{eyepiece}} = -\frac{L}{f_o}\cdot\frac{25}{f_e}$

**Refracting telescope:** $M = -\frac{f_o}{f_e}$ (angular magnification)

---

## 4 | Common Problem Types

### Type 1: Snell's Law
> Light passes from air ($n = 1$) into glass ($n = 1.5$) at 30°. Find the refraction angle.

**Solution:**

$$\sin\theta_2 = \frac{n_1 \sin\theta_1}{n_2} = \frac{1 \times \sin 30°}{1.5} = \frac{0.5}{1.5} = 0.333$$

$$\theta_2 = \sin^{-1}(0.333) \approx 19.5°$$

### Type 2: Critical Angle
> Find the critical angle for water ($n = 1.33$) to air ($n = 1$).

**Solution:**

$$\sin\theta_c = \frac{1}{1.33} = 0.752, \quad \theta_c \approx 48.8°$$

### Type 3: Thin Lens Equation
> A converging lens has $f = 10$ cm. An object is placed 30 cm away. Find $d_i$ and $M$.

**Solution:**

$$\frac{1}{d_i} = \frac{1}{f} - \frac{1}{d_o} = \frac{1}{10} - \frac{1}{30} = \frac{3 - 1}{30} = \frac{2}{30}$$

$$d_i = 15 \text{ cm (real)}, \quad M = -\frac{15}{30} = -0.5$$

Image is real, inverted, half-size.

### Type 4: Concave Mirror
> A concave mirror has $f = 20$ cm. An object is at 15 cm. Find $d_i$ and describe the image.

**Solution:**

$$\frac{1}{d_i} = \frac{1}{20} - \frac{1}{15} = \frac{3 - 4}{60} = -\frac{1}{60}$$

$$d_i = -60 \text{ cm (virtual)}, \quad M = -\frac{-60}{15} = 4$$

Image is virtual, upright, magnified 4× (like a shaving mirror).

---

## 5 | Cross-Links

- [[15_Electromagnetic_Waves]] — Light is an EM wave; refractive index relates to speed
- [[17_Wave_Optics]] — Wave nature of light: interference, diffraction, polarization
- [[09_Sound]] — Similar wave concepts, but light needs no medium
- [[Fundamental/08_Waves]] — Wave properties apply to light propagation
