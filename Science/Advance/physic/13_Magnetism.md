---
tags:
  - physics
  - advance
  - magnetism
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว302"]
---

# Magnetism — แม่เหล็กไฟฟ้า

> *"Magnetism, electricity, and light are but different manifestations of the same fundamental force."* — James Clerk Maxwell

Magnetism arises from moving electric charges. A magnetic field exerts forces on other moving charges and on current-carrying conductors. The Biot-Savart law and Ampère's law provide the tools for calculating magnetic fields from current distributions. The force on a charged particle in a magnetic field leads to circular motion — the basis of mass spectrometers and particle accelerators. The Earth's magnetic field protects life from solar radiation and enables navigation.

In ว302, magnetism completes the static picture: electrostatics describes charges at rest, while magnetism describes charges in motion. Together they set the stage for electromagnetic induction and Maxwell's equations, which unify electricity and magnetism into a single framework.

---

## 1 | Course Coverage

### ม.5 (ว302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Magnetic fields, force on charges/currents, Biot-Savart, Ampère's law, solenoids, Earth's field | Calculate magnetic force; apply Biot-Savart & Ampère's law; solenoid fields |
| **Semester 2** | (Continued in EM induction) | — |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| สนามแม่เหล็ก | Magnetic field | $\vec{B}$ (T) |
| ฟลักซ์แม่เหล็ก | Magnetic flux | $\Phi_B$ (Wb) |
| กฎมือขวา | Right-hand rule | Direction of $\vec{B}$ |
| แรงลอเรนตซ์ | Lorentz force | $\vec{F} = q\vec{v}\times\vec{B}$ |
| กฎบิโอ–ซาวาร์ต | Biot-Savart law | $d\vec{B} = \frac{\mu_0 I \, d\vec{l} \times \hat{r}}{4\pi r^2}$ |
| กฎของแอมแปร์ | Ampère's law | $\oint \vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}}$ |
| ขดลวดโซลีนอยด์ | Solenoid | $B = \mu_0 nI$ |
| สนามแม่เหล็กโลก | Earth's magnetic field | $\approx 25$–$65\,\mu\text{T}$ |
| โมเมนต์แม่เหล็ก | Magnetic dipole moment | $\vec{m}$ (A·m²) |
| ค่าคงตัวแม่เหล็ก | Permeability of free space | $\mu_0 = 4\pi\times 10^{-7}$ T·m/A |
| สารแม่เหล็ก | Magnetic materials | Ferro-, para-, dia-magnetic |

---

## 3 | Key Concepts

### 3.1 Magnetic Force on a Moving Charge

The Lorentz force:

$$\vec{F} = q\vec{v}\times\vec{B}$$

Magnitude: $F = qvB\sin\theta$. The force is perpendicular to both $\vec{v}$ and $\vec{B}$, causing circular motion for charges moving perpendicular to $\vec{B}$.

Radius of circular motion: $r = \frac{mv}{qB}$

Period: $T = \frac{2\pi m}{qB}$

### 3.2 Force on a Current-Carrying Wire

$$\vec{F} = I\vec{L}\times\vec{B}$$

Magnitude: $F = ILB\sin\theta$. Two parallel wires carrying currents $I_1$ and $I_2$ separated by $d$:

$$\frac{F}{L} = \frac{\mu_0 I_1 I_2}{2\pi d}$$

Same-direction currents attract; opposite-direction currents repel.

### 3.3 Biot-Savart Law

Magnetic field from a current element:

$$d\vec{B} = \frac{\mu_0}{4\pi}\frac{I \, d\vec{l}\times\hat{r}}{r^2}$$

**Long straight wire:** $B = \frac{\mu_0 I}{2\pi r}$

**Center of circular loop:** $B = \frac{\mu_0 I}{2R}$

### 3.4 Ampère's Law

$$\oint \vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}}$$

**Solenoid (ideal, long):** $B = \mu_0 nI$ where $n = N/L$ is turns per unit length.

**Toroid:** $B = \frac{\mu_0 NI}{2\pi r}$

### 3.5 Magnetic Dipole Moment

A current loop has magnetic moment $\vec{m} = I\vec{A}$ (where $\vec{A}$ is area vector). Torque in a field:

$$\vec{\tau} = \vec{m}\times\vec{B}$$

Potential energy: $U = -\vec{m}\cdot\vec{B}$

### 3.6 Earth's Magnetic Field

The Earth's field resembles a dipole, with the magnetic south pole near the geographic north pole. The field has components: horizontal (for compass direction) and vertical (dip). The field deflects charged particles from the solar wind, creating the magnetosphere and auroras.

---

## 4 | Common Problem Types

### Type 1: Force on a Moving Charge
> A proton ($q = 1.6 \times 10^{-19}$ C) moves at $2 \times 10^6$ m/s perpendicular to a 0.5 T field. Find the force and radius.

**Solution:**

$$F = qvB = (1.6 \times 10^{-19})(2 \times 10^6)(0.5) = 1.6 \times 10^{-13} \text{ N}$$

$$r = \frac{mv}{qB} = \frac{(1.67 \times 10^{-27})(2 \times 10^6)}{(1.6 \times 10^{-19})(0.5)} = 0.0418 \text{ m}$$

### Type 2: Field from a Wire
> Find $B$ at 0.1 m from a long wire carrying 10 A.

**Solution:**

$$B = \frac{\mu_0 I}{2\pi r} = \frac{(4\pi \times 10^{-7})(10)}{2\pi(0.1)} = 2 \times 10^{-5} \text{ T} = 20\,\mu\text{T}$$

### Type 3: Solenoid Field
> A solenoid has 500 turns over 0.25 m and carries 2 A. Find $B$.

**Solution:**

$$B = \mu_0 nI = (4\pi \times 10^{-7})\left(\frac{500}{0.25}\right)(2) = 5.03 \times 10^{-3} \text{ T}$$

### Type 4: Force Between Parallel Wires
> Two parallel wires 0.05 m apart carry 5 A each in the same direction. Find force per unit length.

**Solution:**

$$\frac{F}{L} = \frac{\mu_0 I_1 I_2}{2\pi d} = \frac{(4\pi \times 10^{-7})(5)(5)}{2\pi(0.05)} = 10^{-4} \text{ N/m (attractive)}$$

---

## 5 | Cross-Links

- [[11_Electrostatics]] — Moving charges create both electric and magnetic fields
- [[12_Electric_Circuits]] — Currents in wires produce magnetic fields
- [[14_Electromagnetic_Induction]] — Changing magnetic fields induce EMF (Faraday's law)
- [[15_Electromagnetic_Waves]] — Oscillating charges produce EM waves
- [[Fundamental/06_Gravity]] — Field concept parallels gravitational fields
