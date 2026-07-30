---
tags:
  - physics
  - advance
  - momentum
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Momentum — โมเมนตัม

> *"In any collision, the universe keeps a perfect accounting of momentum."* — Adapted from Newton's Principia

Momentum (โมเมนตัม) is a vector quantity that captures the "quantity of motion" of an object — the product of its mass and velocity. The **law of conservation of momentum** is one of the most fundamental principles in physics: in the absence of external forces, the total momentum of a system remains constant. This law holds even in collisions where kinetic energy is lost, and even in subatomic and relativistic regimes where Newtonian mechanics fails.

This note covers linear momentum, impulse, the impulse-momentum theorem, conservation of momentum, and elastic, inelastic, and perfectly inelastic collisions in one and two dimensions. Combined with energy analysis, momentum conservation provides a complete toolkit for analysing interactions between objects.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Linear momentum, impulse, impulse-momentum theorem, conservation, elastic/inelastic collisions, 2D collisions | Apply conservation of momentum, classify collision types, solve 1D and 2D collision problems |
| **Semester 2** | (Referenced in wave superposition) | Understand momentum transfer in interactions |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| โมเมนตัมเชิงเส้น | Linear momentum | $\vec{p} = m\vec{v}$ (kg·m/s) |
| แรงกระตุ้น | Impulse | $\vec{J} = \vec{F}\Delta t$ (N·s) |
| การชน | Collision | Interaction of two bodies |
| การชนกึ่งยืดหยุ่น | Elastic collision | KE conserved |
| การชนกึ่งไม่ยืดหยุ่น | Inelastic collision | KE not conserved |
| การชนไม่ยืดหยุ่นสมบูรณ์ | Perfectly inelastic | Objects stick together |
| การอนุรักษ์โมเมนตัม | Conservation of momentum | $\sum \vec{p}_i = \sum \vec{p}_f$ |
| ระบบ | System | Collection of objects |
| แรงภายนอก | External force | Changes total momentum |
| แรงภายใน | Internal force | Cannot change total momentum |

---

## 3 | Key Concepts

### 3.1 Linear Momentum

$$\vec{p} = m\vec{v}$$

Momentum is a **vector** in the direction of velocity. SI unit: kg·m/s.

### 3.2 Impulse and the Impulse-Momentum Theorem

**Impulse** is the product of a force and the time over which it acts:

$$\vec{J} = \vec{F}\Delta t$$

For a variable force, $J = \int F\,dt$, which is the area under a force-time graph.

**Impulse-momentum theorem:**
$$\vec{J} = \Delta \vec{p} = m\vec{v}_f - m\vec{v}_i$$

This explains why airbags and crumple zones work: extending $\Delta t$ reduces the force for a given change in momentum.

### 3.3 Conservation of Momentum

When the net **external** force on a system is zero (an **isolated system**), total momentum is conserved:

$$\sum \vec{p}_i = \sum \vec{p}_f$$

Internal forces (between objects in the system) always cancel by Newton's third law and cannot change the total momentum.

### 3.4 Types of Collisions

| Type | Momentum | Kinetic Energy |
|---|---|---|
| Elastic | Conserved | Conserved |
| Inelastic | Conserved | Not conserved |
| Perfectly inelastic | Conserved | Maximum KE lost; objects stick |

### 3.5 Elastic Collision (1D)

For two masses $m_1, m_2$ with initial velocities $u_1, u_2$:

$$m_1 u_1 + m_2 u_2 = m_1 v_1 + m_2 v_2$$
$$\frac{1}{2}m_1 u_1^2 + \frac{1}{2}m_2 u_2^2 = \frac{1}{2}m_1 v_1^2 + \frac{1}{2}m_2 v_2^2$$

Special cases:
- $m_1 = m_2$: velocities are exchanged ($v_1 = u_2$, $v_2 = u_1$)
- $m_2$ at rest and $m_1 \ll m_2$: $m_1$ rebounds, $m_2$ barely moves

### 3.6 Perfectly Inelastic Collision (1D)

Objects stick together with common final velocity $v$:

$$m_1 u_1 + m_2 u_2 = (m_1 + m_2)v$$
$$v = \frac{m_1 u_1 + m_2 u_2}{m_1 + m_2}$$

Kinetic energy lost:
$$\Delta KE = \frac{1}{2}\frac{m_1 m_2}{m_1 + m_2}(u_1 - u_2)^2$$

### 3.7 2D Collisions

Momentum is conserved **in each component direction**:

$$\sum p_{ix} = \sum p_{fx}, \qquad \sum p_{iy} = \sum p_{fy}$$

Decompose velocities into $x$ and $y$ components and apply conservation to each.

### 3.8 Center of Mass

The center of mass velocity of an isolated system is constant:

$$\vec{v}_{cm} = \frac{\sum m_i \vec{v}_i}{\sum m_i}$$

---

## 4 | Common Problem Types

### Type 1: Perfectly inelastic collision
> A $2\ \text{kg}$ cart at $5\ \text{m/s}$ hits a stationary $3\ \text{kg}$ cart and they stick. Find final velocity.

**Solution:**
$$v = \frac{m_1 u_1 + m_2 u_2}{m_1 + m_2} = \frac{2 \times 5 + 3 \times 0}{5} = 2\ \text{m/s}$$

### Type 2: Impulse from a force-time graph
> A force of $200\ \text{N}$ acts for $0.05\ \text{s}$ on a $0.5\ \text{kg}$ ball at rest. Find final velocity.

**Solution:**
$$J = F\Delta t = 200 \times 0.05 = 10\ \text{N·s}$$
$$\Delta p = J \Rightarrow mv_f = 10 \Rightarrow v_f = \frac{10}{0.5} = 20\ \text{m/s}$$

### Type 3: Elastic collision — equal masses
> A $1\ \text{kg}$ ball at $4\ \text{m/s}$ strikes a stationary $1\ \text{kg}$ ball elastically. Find final velocities.

**Solution:** Equal masses exchange velocities:
$$v_1 = 0\ \text{m/s}, \quad v_2 = 4\ \text{m/s}$$

### Type 4: 2D collision
> A $2\ \text{kg}$ puck at $3\ \text{m/s}$ east strikes a stationary $1\ \text{kg}$ puck. After collision, the $1\ \text{kg}$ puck moves north at $4\ \text{m/s}$. Find the $2\ \text{kg}$ puck's velocity components.

**Solution:** Conserve each component (east = x, north = y):
- x: $2(3) + 0 = 2v_{1x} + 1(0) \Rightarrow v_{1x} = 3\ \text{m/s}$
- y: $0 + 0 = 2v_{1y} + 1(4) \Rightarrow v_{1y} = -2\ \text{m/s}$

---

## 5 | Cross-Links

- [[03_Dynamics]] — Newton's third law underlies momentum conservation
- [[04_Work_Energy_and_Power]] — energy analysis distinguishes collision types
- [[06_Rotational_Motion]] — angular momentum is the rotational analogue
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — vectors, simultaneous equations
