---
tags:
  - mathematics
  - advance
  - vectors
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค302"]
---

# Vectors — เวกเตอร์

> *"Vectors are arrows with attitude — they carry both magnitude and direction, the language of physics and computer graphics."*

Vectors represent quantities with both magnitude and direction, essential for physics (forces, velocities), engineering (stress analysis), and computer science (3D graphics, machine learning). This topic covers vector operations, dot and cross products, and applications to geometry and physics.

---

## 1 | Course Coverage

### ม.5 (ค302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Vector basics | Definition; magnitude; direction; unit vectors; position vectors |
| **Semester 1** | Vector operations | Addition, subtraction, scalar multiplication; component form |
| **Semester 1** | Dot product | Definition; geometric interpretation; angle between vectors; projection |
| **Semester 1** | Cross product | Definition; geometric interpretation; area of parallelogram; normal vectors |
| **Semester 1** | 3D vectors | Extension to three dimensions; applications |
| **Semester 1** | Applications | Force vectors; work; torque; lines and planes in 3D |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| เวกเตอร์ | Vector | $\vec{v}$ or $\mathbf{v}$ |
| สเกลาร์ | Scalar | Real number |
| ขนาด | Magnitude | $|\vec{v}|$ or $\|\vec{v}\|$ |
| ทิศทาง | Direction | Angle $\theta$ |
| เวกเตอร์หนึ่งหน่วย | Unit vector | $\hat{v}$ |
| ผลคูณเชิงสเกลาร์ | Dot product | $\vec{u} \cdot \vec{v}$ |
| ผลคูณเชิงเวกเตอร์ | Cross product | $\vec{u} \times \vec{v}$ |
| การฉาย | Projection | $\text{proj}_{\vec{u}} \vec{v}$ |
| เวกเตอร์ปกติ | Normal vector | $\vec{n}$ |

---

## 3 | Key Concepts

### 3.1 Vector Definition

A **vector** has magnitude and direction. In component form:
$$\vec{v} = \langle v_x, v_y \rangle = v_x \hat{i} + v_y \hat{j}$$

**Magnitude:**
$$|\vec{v}| = \sqrt{v_x^2 + v_y^2}$$

**Direction (angle from positive x-axis):**
$$\theta = \tan^{-1}\left(\frac{v_y}{v_x}\right)$$

**Unit vector:**
$$\hat{v} = \frac{\vec{v}}{|\vec{v}|}$$

### 3.2 Vector Operations

**Addition:**
$$\vec{u} + \vec{v} = \langle u_x + v_x, u_y + v_y \rangle$$

**Subtraction:**
$$\vec{u} - \vec{v} = \langle u_x - v_x, u_y - v_y \rangle$$

**Scalar multiplication:**
$$c\vec{v} = \langle cv_x, cv_y \rangle$$

### 3.3 Dot Product

**Algebraic definition:**
$$\vec{u} \cdot \vec{v} = u_x v_x + u_y v_y$$

**Geometric definition:**
$$\vec{u} \cdot \vec{v} = |\vec{u}||\vec{v}|\cos\theta$$

**Angle between vectors:**
$$\cos\theta = \frac{\vec{u} \cdot \vec{v}}{|\vec{u}||\vec{v}|}$$

**Properties:**
- Commutative: $\vec{u} \cdot \vec{v} = \vec{v} \cdot \vec{u}$
- $\vec{u} \cdot \vec{u} = |\vec{u}|^2$
- Perpendicular vectors: $\vec{u} \cdot \vec{v} = 0$

**Projection of $\vec{v}$ onto $\vec{u}$:**
$$\text{proj}_{\vec{u}} \vec{v} = \frac{\vec{u} \cdot \vec{v}}{|\vec{u}|^2} \vec{u}$$

### 3.4 Cross Product (3D only)

**Definition:**
$$\vec{u} \times \vec{v} = \langle u_y v_z - u_z v_y, u_z v_x - u_x v_z, u_x v_y - u_y v_x \rangle$$

**Determinant form:**
$$\vec{u} \times \vec{v} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ u_x & u_y & u_z \\ v_x & v_y & v_z \end{vmatrix}$$

**Geometric interpretation:**
- Magnitude: $|\vec{u} \times \vec{v}| = |\vec{u}||\vec{v}|\sin\theta$ = area of parallelogram
- Direction: perpendicular to both $\vec{u}$ and $\vec{v}$ (right-hand rule)

**Properties:**
- Anti-commutative: $\vec{u} \times \vec{v} = -(\vec{v} \times \vec{u})$
- $\vec{u} \times \vec{u} = \vec{0}$
- Parallel vectors: $\vec{u} \times \vec{v} = \vec{0}$

### 3.5 Applications

**Work done by a force:**
$$W = \vec{F} \cdot \vec{d}$$

**Torque:**
$$\vec{\tau} = \vec{r} \times \vec{F}$$

**Area of triangle:**
$$\text{Area} = \frac{1}{2}|\vec{u} \times \vec{v}|$$

**Volume of parallelepiped:**
$$V = |\vec{u} \cdot (\vec{v} \times \vec{w})|$$

### 3.6 Lines and Planes in 3D

**Line (parametric form):**
$$\vec{r}(t) = \vec{r}_0 + t\vec{v}$$
$$x = x_0 + at, \quad y = y_0 + bt, \quad z = z_0 + ct$$

**Plane:**
$$\vec{n} \cdot (\vec{r} - \vec{r}_0) = 0$$
$$a(x - x_0) + b(y - y_0) + c(z - z_0) = 0$$
where $\vec{n} = \langle a, b, c \rangle$ is the normal vector.

---

## 4 | Common Problem Types

### Type 1: Vector Magnitude and Direction
> Find magnitude and direction of $\vec{v} = \langle 3, -4 \rangle$.

**Solution:** $|\vec{v}| = \sqrt{9 + 16} = 5$
$\theta = \tan^{-1}(-4/3) \approx -53.1°$ or $306.9°$

### Type 2: Dot Product and Angle
> Find angle between $\vec{u} = \langle 1, 2 \rangle$ and $\vec{v} = \langle 3, 1 \rangle$.

**Solution:** $\vec{u} \cdot \vec{v} = 3 + 2 = 5$
$|\vec{u}| = \sqrt{5}$, $|\vec{v}| = \sqrt{10}$
$\cos\theta = \frac{5}{\sqrt{50}} = \frac{5}{5\sqrt{2}} = \frac{1}{\sqrt{2}}$
$\theta = 45°$

### Type 3: Cross Product
> Compute $\vec{u} \times \vec{v}$ where $\vec{u} = \langle 1, 2, 3 \rangle$, $\vec{v} = \langle 4, 5, 6 \rangle$.

**Solution:** $\vec{u} \times \vec{v} = \langle (2)(6)-(3)(5), (3)(4)-(1)(6), (1)(5)-(2)(4) \rangle$
$= \langle 12-15, 12-6, 5-8 \rangle = \langle -3, 6, -3 \rangle$

### Type 4: Work
> A force $\vec{F} = \langle 10, 5 \rangle$ N moves an object by $\vec{d} = \langle 8, 2 \rangle$ m. Find work done.

**Solution:** $W = \vec{F} \cdot \vec{d} = 80 + 10 = 90$ J

### Type 5: Plane Equation
> Find equation of plane through $(1, 2, 3)$ with normal $\vec{n} = \langle 2, -1, 4 \rangle$.

**Solution:** $2(x-1) - 1(y-2) + 4(z-3) = 0$
$2x - y + 4z = 12$

---

## 5 | Cross-Links

- [[07_Trigonometric_Functions]] — Direction angles
- [[11_Matrices_and_Determinants]] — Cross product via determinant
- [[15_Differentiation]] — Gradient vectors
- [[01_Physics - Overview]] — Force, velocity, acceleration vectors
