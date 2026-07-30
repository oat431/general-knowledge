---
tags:
  - physics
  - advance
  - special-relativity
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว303"]
---

# Special Relativity — ทฤษฎีสัมพัทธภาพพิเศษ

> *"Put your hand on a hot stove for a minute, and it seems like an hour. Sit with a pretty girl for an hour, and it seems like a minute. THAT'S relativity."* — Albert Einstein

Special relativity, published by Albert Einstein in 1905, revolutionized our understanding of space and time. It discards the notion of absolute time inherited from Newtonian mechanics and establishes that space and time are interwoven into a single four-dimensional continuum called spacetime. The theory is built on two simple postulates yet yields profound consequences: moving clocks run slow, moving rods shrink, and mass is a form of energy.

For Thai high school physics (ว303), students focus on the kinematic consequences of the theory — time dilation, length contraction, relativistic momentum, and mass-energy equivalence — along with an introduction to Lorentz transformations. Mastery of these concepts lays the groundwork for understanding modern particle physics and cosmology.

---

## 1 | Course Coverage

### ม.6 (ว303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Postulates of special relativity, Galilean vs Lorentz transformations, time dilation, length contraction | Apply Lorentz factor γ; calculate dilated time and contracted length; distinguish proper vs measured quantities |
| **Semester 2** | Relativistic momentum, mass-energy equivalence E=mc², relativistic energy, velocity addition | Solve relativistic collision problems; compute total energy and kinetic energy; apply relativistic velocity addition |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| สัมพัทธภาพพิเศษ | Special relativity | Theory restricted to inertial frames |
| กรอบอ้างอิงเฉื่อย | Inertial reference frame | Frame moving at constant velocity |
| หลักการสัมพัทธภาพ | Principle of relativity | Laws of physics same in all inertial frames |
| ความเร็วแสงคงที่ | Constancy of speed of light | c = 299,792,458 m/s ≈ 3.00×10⁸ m/s |
| ตัวประกอบลอเรนซ์ | Lorentz factor | $\gamma = \frac{1}{\sqrt{1 - v^2/c^2}}$ |
| การขยายเวลา | Time dilation | Moving clock runs slow |
| การหดสั้นความยาว | Length contraction | Moving rod shrinks along motion |
| มวล-พลังงานสมมูล | Mass-energy equivalence | $E = mc^2$ |
| โมเมนตัมเชิงสัมพัทธภาพ | Relativistic momentum | $p = \gamma m v$ |
| พลังงานนิ่ง | Rest energy | $E_0 = m_0 c^2$ |
| เหตุการณ์ | Event | Point in spacetime (x, y, z, t) |
| เวลาในตัว | Proper time | $\Delta t_0$, time measured in rest frame |
| ความยาวในตัว | Proper length | $L_0$, length measured in rest frame |

---

## 3 | Key Concepts

### 3.1 The Two Postulates

1. **Principle of relativity (หลักการสัมพัทธภาพ):** The laws of physics have the same form in all inertial reference frames. No experiment can distinguish one inertial frame from another.
2. **Constancy of the speed of light (ความเร็วแสงคงที่):** The speed of light in vacuum $c$ is the same for all inertial observers, regardless of the motion of the source or observer.

### 3.2 Galilean vs Lorentz Transformation

For a frame $S'$ moving at velocity $v$ along the x-axis of frame $S$:

**Galilean (classical, valid only for $v \ll c$):**

$$x' = x - vt, \quad t' = t$$

**Lorentz (relativistic, valid for all $v < c$):**

$$x' = \gamma(x - vt), \quad t' = \gamma\left(t - \frac{vx}{c^2}\right)$$

where the Lorentz factor is

$$\gamma = \frac{1}{\sqrt{1 - \frac{v^2}{c^2}}}$$

Note that $\gamma \geq 1$, with $\gamma \to \infty$ as $v \to c$.

### 3.3 Time Dilation

A clock moving relative to an observer ticks slower. If $\Delta t_0$ is the **proper time** (measured in the clock's rest frame), the time observed in a frame where the clock moves at speed $v$ is:

$$\Delta t = \gamma \, \Delta t_0$$

Since $\gamma > 1$, we always have $\Delta t > \Delta t_0$ — the moving clock appears to run slow.

### 3.4 Length Contraction

An object moving relative to an observer appears shortened **along the direction of motion**. If $L_0$ is the **proper length** (measured in the object's rest frame):

$$L = \frac{L_0}{\gamma} = L_0 \sqrt{1 - \frac{v^2}{c^2}}$$

Perpendicular dimensions are unaffected — contraction occurs only along the direction of relative motion.

### 3.5 Relativistic Momentum

Classical momentum $p = mv$ fails at high speeds. The relativistic momentum is:

$$p = \gamma m_0 v = \frac{m_0 v}{\sqrt{1 - v^2/c^2}}$$

where $m_0$ is the **rest mass**. As $v \to c$, $p \to \infty$, which explains why no massive object can reach the speed of light — it would require infinite momentum (and infinite energy).

### 3.6 Mass-Energy Equivalence

Einstein's most famous result states that mass and energy are interchangeable:

$$E = mc^2$$

For a particle at rest, this gives the **rest energy** $E_0 = m_0 c^2$. The total relativistic energy is:

$$E = \gamma m_0 c^2 = \sqrt{(pc)^2 + (m_0 c^2)^2}$$

The relativistic kinetic energy is:

$$K = E - E_0 = (\gamma - 1) m_0 c^2$$

This reduces to the classical $\frac{1}{2}mv^2$ when $v \ll c$.

### 3.7 Relativistic Velocity Addition

If an object moves at speed $u'$ in frame $S'$, which moves at speed $v$ relative to $S$, the speed in $S$ is:

$$u = \frac{u' + v}{1 + \frac{u' v}{c^2}}$$

This guarantees that no composition of velocities exceeds $c$.

---

## 4 | Common Problem Types

### Type 1: Time dilation calculation
> A muon (มิวออน) is created at 10 km altitude and travels toward Earth at 0.98c. Its proper lifetime is 2.2 μs. Will it reach the ground?

**Solution:**

Step 1 — Compute Lorentz factor:

$$\gamma = \frac{1}{\sqrt{1 - 0.98^2}} = \frac{1}{\sqrt{1 - 0.9604}} = \frac{1}{\sqrt{0.0396}} \approx 5.03$$

Step 2 — Dilated lifetime in Earth frame:

$$\Delta t = \gamma \, \Delta t_0 = 5.03 \times 2.2 \ \mu\text{s} \approx 11.1 \ \mu\text{s}$$

Step 3 — Distance traveled: $d = v \Delta t = 0.98 \times 3 \times 10^8 \times 11.1 \times 10^{-6} \approx 3260 \ \text{m}$

From Earth's perspective, the muon travels ~3.3 km — not quite 10 km. But in the muon's frame, the atmosphere is **length-contracted**: $L = 10000/5.03 \approx 1990$ m, which it covers in its 2.2 μs lifetime. ✓

---

### Type 2: Mass-energy conversion
> Find the energy released when 1 gram of matter is completely converted to energy.

**Solution:**

$$E = mc^2 = (0.001 \ \text{kg})(3.00 \times 10^8 \ \text{m/s})^2 = 9.00 \times 10^{13} \ \text{J}$$

That is about 25,000 MWh — enough to power a small city for a day.

---

### Type 3: Relativistic momentum and energy
> A proton (rest mass $1.67 \times 10^{-27}$ kg) moves at 0.85c. Find its total energy, kinetic energy, and momentum.

**Solution:**

$$\gamma = \frac{1}{\sqrt{1 - 0.85^2}} = \frac{1}{\sqrt{0.2775}} \approx 1.898$$

$$E_0 = m_0 c^2 = (1.67 \times 10^{-27})(9 \times 10^{16}) \approx 1.503 \times 10^{-10} \ \text{J} \approx 938 \ \text{MeV}$$

$$E = \gamma E_0 \approx 1.898 \times 938 \approx 1780 \ \text{MeV}$$

$$K = (\gamma - 1) m_0 c^2 \approx 0.898 \times 938 \approx 842 \ \text{MeV}$$

$$p = \gamma m_0 v = 1.898 \times 1.67 \times 10^{-27} \times 0.85 \times 3 \times 10^8 \approx 8.05 \times 10^{-19} \ \text{kg·m/s}$$

---

## 5 | Cross-Links

- [[17_Electromagnetic_Waves]] — Maxwell's equations predict c, motivating the second postulate
- [[19_Quantum_Physics]] — Relativistic quantum mechanics extends SR to quantum particles
- [[21_Nuclear_Physics]] — Mass-energy equivalence explains nuclear binding energy and fission/fusion energy
- [[23_Astrophysics_and_Cosmology]] — Relativistic effects are crucial in high-energy astrophysical phenomena
