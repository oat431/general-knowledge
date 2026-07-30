---
tags:
  - physics
  - advance
  - rotational-motion
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Rotational Motion — การเคลื่อนที่แบบหมุน

> *"Everything turns, and everything rolls; the universe itself is a great spinning wheel."* — Adapted from classical mechanics

Rotational motion (การเคลื่อนที่แบบหมุน) extends the linear mechanics of the previous topics to objects that rotate about an axis. Every linear quantity has a rotational analogue: displacement becomes angle, velocity becomes angular velocity, force becomes torque, mass becomes moment of inertia, and momentum becomes angular momentum. The same Newton's laws, energy principles, and conservation laws apply — just rewritten in angular form. This parallel structure makes rotational motion both elegant and powerful.

This note covers angular kinematics, torque, moment of inertia, rotational dynamics ($\tau = I\alpha$), rotational kinetic energy, angular momentum and its conservation, and rolling without slipping. These concepts are essential for understanding wheels, gears, pulleys, gyroscopes, and planetary motion.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Angular displacement/velocity/acceleration, torque, moment of inertia, rotational dynamics, rotational KE, angular momentum, rolling motion | Solve rotational kinematics, apply $\tau = I\alpha$, use angular momentum conservation |
| **Semester 2** | (Applied in oscillations — torque causes SHM) | Relate torque to restoring motion in pendulums |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| มุม | Angle | $\theta$ (rad) |
| ความเร็วเชิงมุม | Angular velocity | $\omega$ (rad/s) |
| ความเร่งเชิงมุม | Angular acceleration | $\alpha$ (rad/s²) |
| ทอร์ก / ทรงบิด | Torque | $\tau = rF\sin\theta$ (N·m) |
| โมเมนต์ความเฉื่อย | Moment of inertia | $I$ (kg·m²) |
| พลังงานจลน์เชิงหมุน | Rotational KE | $KE_{rot} = \frac{1}{2}I\omega^2$ |
| โมเมนตัมเชิงมุม | Angular momentum | $L = I\omega$ (kg·m²/s) |
| การกลิ้ง | Rolling | $v = r\omega$ |
| จุดศูนย์กลางมวล | Center of mass | Point of average mass |

---

## 3 | Key Concepts

### 3.1 Angular Kinematics

For constant angular acceleration $\alpha$:

| Equation | Form |
|---|---|
| 1 | $\omega = \omega_0 + \alpha t$ |
| 2 | $\theta = \theta_0 + \omega_0 t + \frac{1}{2}\alpha t^2$ |
| 3 | $\omega^2 = \omega_0^2 + 2\alpha(\theta - \theta_0)$ |

Relationship to linear quantities (at radius $r$):

| Linear | Angular | Relation |
|---|---|---|
| Arc length $s$ | Angle $\theta$ | $s = r\theta$ |
| Tangential velocity $v$ | Angular velocity $\omega$ | $v = r\omega$ |
| Tangential acceleration $a_t$ | Angular acceleration $\alpha$ | $a_t = r\alpha$ |
| Centripetal acceleration $a_c$ | — | $a_c = r\omega^2 = \frac{v^2}{r}$ |

### 3.2 Torque

Torque is the rotational analogue of force — the tendency to cause rotation:

$$\tau = rF\sin\theta$$

where $r$ is the lever arm, $F$ the force, and $\theta$ the angle between them. When the force is perpendicular, $\tau = rF$.

### 3.3 Moment of Inertia

Moment of inertia (โมเมนต์ความเฉื่อย) measures resistance to angular acceleration:

$$I = \sum m_i r_i^2 \quad \text{or} \quad I = \int r^2\,dm$$

Common shapes (about center of mass):

| Object | Moment of Inertia |
|---|---|
| Point mass at radius $r$ | $I = mr^2$ |
| Solid disk / cylinder | $I = \frac{1}{2}mr^2$ |
| Hoop / ring | $I = mr^2$ |
| Solid sphere | $I = \frac{2}{5}mr^2$ |
| Long rod (center) | $I = \frac{1}{12}mL^2$ |
| Long rod (end) | $I = \frac{1}{3}mL^2$ |

**Parallel axis theorem:**
$$I = I_{cm} + Md^2$$

### 3.4 Rotational Dynamics (Newton's Second Law)

$$\sum \tau = I\alpha$$

### 3.5 Rotational Kinetic Energy

$$KE_{rot} = \frac{1}{2}I\omega^2$$

Total KE of a rolling object:
$$KE_{total} = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$$

### 3.6 Angular Momentum

$$L = I\omega$$

**Conservation of angular momentum:** When net external torque is zero:
$$I_i \omega_i = I_f \omega_f$$

Example: figure skater pulling arms in — $I$ decreases, so $\omega$ increases.

### 3.7 Rolling Without Slipping

For pure rolling: $v_{cm} = r\omega$. The contact point is instantaneously at rest.

---

## 4 | Common Problem Types

### Type 1: Torque and equilibrium
> A $10\ \text{N}$ force is applied perpendicular to a $0.5\ \text{m}$ wrench. Find torque.

**Solution:**
$$\tau = rF = 0.5 \times 10 = 5\ \text{N·m}$$

### Type 2: Rotational dynamics
> A solid disk ($m = 2\ \text{kg}$, $r = 0.3\ \text{m}$) experiences a torque of $3\ \text{N·m}$. Find angular acceleration.

**Solution:**
$$I = \frac{1}{2}mr^2 = \frac{1}{2}(2)(0.09) = 0.09\ \text{kg·m}^2$$
$$\alpha = \frac{\tau}{I} = \frac{3}{0.09} = 33.3\ \text{rad/s}^2$$

### Type 3: Conservation of angular momentum
> A skater ($I_i = 4\ \text{kg·m}^2$, $\omega_i = 2\ \text{rad/s}$) pulls arms in to $I_f = 1\ \text{kg·m}^2$. Find $\omega_f$.

**Solution:**
$$I_i \omega_i = I_f \omega_f \Rightarrow \omega_f = \frac{4 \times 2}{1} = 8\ \text{rad/s}$$

### Type 4: Rolling energy
> A solid sphere ($m = 1\ \text{kg}$, $r = 0.2\ \text{m}$) rolls at $v = 4\ \text{m/s}$. Find total KE.

**Solution:**
$$I = \frac{2}{5}mr^2 = \frac{2}{5}(1)(0.04) = 0.016\ \text{kg·m}^2$$
$$\omega = \frac{v}{r} = 20\ \text{rad/s}$$
$$KE = \frac{1}{2}mv^2 + \frac{1}{2}I\omega^2 = \frac{1}{2}(1)(16) + \frac{1}{2}(0.016)(400) = 8 + 3.2 = 11.2\ \text{J}$$

---

## 5 | Cross-Links

- [[03_Dynamics]] — rotational analogues of Newton's laws
- [[04_Work_Energy_and_Power]] — rotational KE extends energy conservation
- [[05_Momentum]] — angular momentum parallels linear momentum
- [[07_Oscillations]] — torque provides restoring force in pendulums
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — integration, geometry
