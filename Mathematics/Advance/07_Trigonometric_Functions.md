---
tags:
  - mathematics
  - advance
  - trigonometry
  - functions
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Trigonometric Functions — ฟังก์ชันตรีโกณมิติ

> *"Trigonometry is the mathematics of cycles, waves, and rotation — the language of periodic phenomena."*

Trigonometric functions extend the basic ratios learned in geometry to functions defined on all real numbers via the unit circle. This topic covers radian measure, the six trig functions, their graphs, identities, and inverse functions — preparing students for calculus and physics applications.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Angle measurement | Degrees and radians; conversion; arc length; sector area |
| **Semester 2** | Unit circle definition | Sine, cosine, tangent on unit circle; coordinates $(\cos\theta, \sin\theta)$ |
| **Semester 2** | All six trig functions | sin, cos, tan, csc, sec, cot; reciprocal identities |
| **Semester 2** | Graphs of trig functions | Amplitude, period, phase shift, vertical shift; transformations |
| **Semester 2** | Fundamental identities | Pythagorean, quotient, reciprocal identities |
| **Semester 2** | Inverse trig functions | $\sin^{-1}$, $\cos^{-1}$, $\tan^{-1}$; restricted domains; principal values |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| เรเดียน | Radian | rad |
| วงกลมหนึ่งหน่วย | Unit circle | Circle of radius 1 |
| ฟังก์ชันไซน์ | Sine function | $\sin\theta$ |
| ฟังก์ชันโคไซน์ | Cosine function | $\cos\theta$ |
| ฟังก์ชันแทนเจนต์ | Tangent function | $\tan\theta$ |
| แอมพลิจูด | Amplitude | $A$ in $A\sin(x)$ |
| คาบ | Period | $T$ |
| การเลื่อนเฟส | Phase shift | $C$ in $\sin(x - C)$ |
| ฟังก์ชันผกผัน | Inverse function | $\sin^{-1}$, $\arcsin$ |
| เอกลักษณ์ | Identity | Equation true for all values |

---

## 3 | Key Concepts

### 3.1 Radian Measure

**Definition:** One radian is the angle subtended by an arc of length equal to the radius.

**Conversion:**
$$\pi \text{ radians} = 180^\circ$$
$$\text{Radians} = \text{Degrees} \times \frac{\pi}{180}$$
$$\text{Degrees} = \text{Radians} \times \frac{180}{\pi}$$

**Common angles:**

| Degrees | Radians |
|---|---|
| 0° | 0 |
| 30° | $\pi/6$ |
| 45° | $\pi/4$ |
| 60° | $\pi/3$ |
| 90° | $\pi/2$ |
| 180° | $\pi$ |
| 270° | $3\pi/2$ |
| 360° | $2\pi$ |

**Arc length:** $s = r\theta$ (where $\theta$ is in radians)

**Sector area:** $A = \frac{1}{2}r^2\theta$

### 3.2 Unit Circle Definition

On the unit circle, for angle $\theta$:
$$\cos\theta = x\text{-coordinate}$$
$$\sin\theta = y\text{-coordinate}$$

**Other trig functions:**
$$\tan\theta = \frac{\sin\theta}{\cos\theta}, \quad \cot\theta = \frac{\cos\theta}{\sin\theta}$$
$$\sec\theta = \frac{1}{\cos\theta}, \quad \csc\theta = \frac{1}{\sin\theta}$$

**Exact values for common angles:**

| $\theta$ | $\sin\theta$ | $\cos\theta$ | $\tan\theta$ |
|---|---|---|---|
| $0$ | $0$ | $1$ | $0$ |
| $\pi/6$ | $1/2$ | $\sqrt{3}/2$ | $\sqrt{3}/3$ |
| $\pi/4$ | $\sqrt{2}/2$ | $\sqrt{2}/2$ | $1$ |
| $\pi/3$ | $\sqrt{3}/2$ | $1/2$ | $\sqrt{3}$ |
| $\pi/2$ | $1$ | $0$ | undefined |

### 3.3 Graphs of Trigonometric Functions

**General form:** $y = A\sin(Bx - C) + D$

| Parameter | Effect |
|---|---|
| $A$ | Amplitude = $\|A\|$ |
| $B$ | Period = $\frac{2\pi}{\|B\|}$ |
| $C$ | Phase shift = $\frac{C}{B}$ (right if positive) |
| $D$ | Vertical shift = $D$ |

**Periods of basic functions:**
- $\sin x$, $\cos x$: period $2\pi$
- $\tan x$, $\cot x$: period $\pi$
- $\sec x$, $\csc x$: period $2\pi$

### 3.4 Fundamental Identities

**Pythagorean identities:**
$$\sin^2\theta + \cos^2\theta = 1$$
$$1 + \tan^2\theta = \sec^2\theta$$
$$1 + \cot^2\theta = \csc^2\theta$$

**Quotient identities:**
$$\tan\theta = \frac{\sin\theta}{\cos\theta}$$
$$\cot\theta = \frac{\cos\theta}{\sin\theta}$$

**Reciprocal identities:**
$$\csc\theta = \frac{1}{\sin\theta}, \quad \sec\theta = \frac{1}{\cos\theta}, \quad \cot\theta = \frac{1}{\tan\theta}$$

**Even-odd identities:**
$$\sin(-\theta) = -\sin\theta \quad \text{(odd)}$$
$$\cos(-\theta) = \cos\theta \quad \text{(even)}$$
$$\tan(-\theta) = -\tan\theta \quad \text{(odd)}$$

### 3.5 Sum and Difference Formulas

$$\sin(A \pm B) = \sin A \cos B \pm \cos A \sin B$$
$$\cos(A \pm B) = \cos A \cos B \mp \sin A \sin B$$
$$\tan(A \pm B) = \frac{\tan A \pm \tan B}{1 \mp \tan A \tan B}$$

### 3.6 Double-Angle Formulas

$$\sin 2\theta = 2\sin\theta\cos\theta$$
$$\cos 2\theta = \cos^2\theta - \sin^2\theta = 2\cos^2\theta - 1 = 1 - 2\sin^2\theta$$
$$\tan 2\theta = \frac{2\tan\theta}{1 - \tan^2\theta}$$

### 3.7 Inverse Trigonometric Functions

| Function | Domain | Range | Meaning |
|---|---|---|---|
| $\sin^{-1} x$ | $[-1, 1]$ | $[-\pi/2, \pi/2]$ | Angle whose sine is $x$ |
| $\cos^{-1} x$ | $[-1, 1]$ | $[0, \pi]$ | Angle whose cosine is $x$ |
| $\tan^{-1} x$ | $\mathbb{R}$ | $(-\pi/2, \pi/2)$ | Angle whose tangent is $x$ |

**Example:** $\sin^{-1}(1/2) = \pi/6$ because $\sin(\pi/6) = 1/2$ and $\pi/6 \in [-\pi/2, \pi/2]$

---

## 4 | Common Problem Types

### Type 1: Degree-Radian Conversion
> Convert $150°$ to radians and $\frac{5\pi}{4}$ to degrees.

**Solution:** $150° \times \frac{\pi}{180} = \frac{5\pi}{6}$
$\frac{5\pi}{4} \times \frac{180}{\pi} = 225°$

### Type 2: Arc Length
> Find the arc length of a circle with radius 6 cm and central angle $75°$.

**Solution:** Convert to radians: $75° = \frac{5\pi}{12}$
$s = r\theta = 6 \times \frac{5\pi}{12} = \frac{5\pi}{2} \approx 7.85$ cm

### Type 3: Exact Values
> Find $\sin(7\pi/6)$ and $\cos(7\pi/6)$.

**Solution:** $7\pi/6 = \pi + \pi/6$ (third quadrant)
Reference angle: $\pi/6$
In Q3, both sin and cos are negative:
$\sin(7\pi/6) = -\sin(\pi/6) = -1/2$
$\cos(7\pi/6) = -\cos(\pi/6) = -\sqrt{3}/2$

### Type 4: Graph Analysis
> Find amplitude, period, and phase shift of $y = 3\sin(2x - \pi/2) + 1$.

**Solution:**
- Amplitude: $|A| = 3$
- Period: $\frac{2\pi}{|B|} = \frac{2\pi}{2} = \pi$
- Phase shift: $\frac{C}{B} = \frac{\pi/2}{2} = \frac{\pi}{4}$ (right)
- Vertical shift: $D = 1$

### Type 5: Identity Verification
> Verify: $\frac{1 - \cos 2\theta}{\sin 2\theta} = \tan\theta$

**Solution:**
$\frac{1 - (1 - 2\sin^2\theta)}{2\sin\theta\cos\theta} = \frac{2\sin^2\theta}{2\sin\theta\cos\theta} = \frac{\sin\theta}{\cos\theta} = \tan\theta$ ✓

### Type 6: Inverse Trig Evaluation
> Find $\cos^{-1}(-\sqrt{2}/2)$.

**Solution:** We need angle in $[0, \pi]$ whose cosine is $-\sqrt{2}/2$.
$\cos(\pi/4) = \sqrt{2}/2$, so $\cos(\pi - \pi/4) = \cos(3\pi/4) = -\sqrt{2}/2$.
**Answer:** $\cos^{-1}(-\sqrt{2}/2) = 3\pi/4$

---

## 5 | Cross-Links

- [[Fundamental/12_Geometry_Shapes]] — Basic angle concepts
- [[09_Trigonometric_Equations]] — Solving trig equations
- [[14_Limits_and_Continuity]] — Limits involving trig functions
- [[15_Differentiation]] — Derivatives of trig functions
- [[13_Vectors]] — Direction angles and components
