---
tags:
  - physics
  - advance
  - kinematics
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Kinematics — อุณหพลศาสตร์

> *"I can calculate the motion of heavenly bodies, but not the madness of people."* — Isaac Newton

Kinematics (อุณหพลศาสตร์) is the study of motion **without** considering its causes. It describes how objects move in terms of displacement, velocity, and acceleration, and it provides the mathematical tools — the kinematic equations — to predict future positions and velocities once the initial state is known. This topic is the foundation of all mechanics: before we ask *why* something moves (dynamics), we must first describe *how* it moves.

This note covers motion in one and two dimensions, including uniform and uniformly accelerated motion, free fall, projectile motion, and graphical analysis of motion. Students must distinguish carefully between displacement and distance, velocity and speed, and understand vectors throughout.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Displacement, velocity, acceleration, kinematic equations, free fall, projectile motion, motion graphs | Solve 1D and 2D motion problems, interpret and draw x-t, v-t, a-t graphs, decompose projectile motion |
| **Semester 2** | (Applied to oscillations and waves) | Relate kinematics to SHM and wave propagation |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| การกระจัด | Displacement | $\vec{s}$ or $\Delta \vec{x}$ (vector) |
| ระยะทาง | Distance | $d$ (scalar) |
| ความเร็ว | Velocity | $\vec{v}$ (vector) |
| อัตราเร็ว | Speed | $v$ (scalar) |
| ความเร่ง | Acceleration | $\vec{a}$ (vector) |
| ความเร่งคงที่ | Uniform acceleration | $a = \text{const}$ |
| ตกอิสระ | Free fall | $g \approx 9.8\ \text{m/s}^2$ |
| การเคลื่อนที่แบบหนึ่งมิติ | 1D motion | Along a line |
| การเคลื่อนที่แบบโพรเจกไทล์ | Projectile motion | 2D under gravity |
| ปริมาณเวกเตอร์ | Vector quantity | Has magnitude + direction |
| ปริมาณสเกลาร์ | Scalar quantity | Has magnitude only |

---

## 3 | Key Concepts

### 3.1 Displacement, Velocity, and Acceleration

**Displacement** is the change in position: $\Delta \vec{x} = \vec{x}_f - \vec{x}_i$. It is a vector; **distance** is the scalar path length.

**Average velocity**:
$$\vec{v}_{avg} = \frac{\Delta \vec{x}}{\Delta t}$$

**Instantaneous velocity**:
$$\vec{v} = \lim_{\Delta t \to 0} \frac{\Delta \vec{x}}{\Delta t} = \frac{d\vec{x}}{dt}$$

**Average and instantaneous acceleration**:
$$\vec{a}_{avg} = \frac{\Delta \vec{v}}{\Delta t}, \qquad \vec{a} = \frac{d\vec{v}}{dt}$$

### 3.2 Kinematic Equations (Constant Acceleration)

For motion with constant acceleration $a$:

| Equation | Relates | Form |
|---|---|---|
| 1 | $v, v_0, a, t$ | $v = v_0 + at$ |
| 2 | $x, x_0, v_0, a, t$ | $x = x_0 + v_0 t + \frac{1}{2}at^2$ |
| 3 | $v^2, v_0^2, a, x$ | $v^2 = v_0^2 + 2a(x - x_0)$ |
| 4 | $x, v_0, v, t$ | $x = x_0 + \frac{1}{2}(v_0 + v)t$ |

### 3.3 Free Fall

Near Earth's surface, gravity gives a constant acceleration (neglecting air resistance):

$$g \approx 9.8\ \text{m/s}^2\ \text{downward}$$

All kinematic equations apply with $a = -g$ (if upward is positive).

### 3.4 Projectile Motion

Decompose motion into **horizontal** (constant velocity) and **vertical** (constant acceleration $g$):

- **Horizontal:** $x = v_{0x}t$, where $v_{0x} = v_0 \cos\theta$
- **Vertical:** $y = v_{0y}t - \frac{1}{2}gt^2$, where $v_{0y} = v_0 \sin\theta$

**Time of flight** (launch and landing at same height):
$$T = \frac{2v_0 \sin\theta}{g}$$

**Maximum range:**
$$R = \frac{v_0^2 \sin 2\theta}{g}$$

Maximum range occurs at $\theta = 45^\circ$.

**Maximum height:**
$$H = \frac{v_0^2 \sin^2\theta}{2g}$$

### 3.5 Motion Graphs

| Graph | Slope | Area under curve |
|---|---|---|
| Position vs time ($x$-$t$) | velocity | — |
| Velocity vs time ($v$-$t$) | acceleration | displacement |
| Acceleration vs time ($a$-$t$) | — | change in velocity |

```mermaid
flowchart LR
    A["Position-time graph"] -->|"slope"| B["Velocity"]
    B -->|"slope"| C["Acceleration"]
    C -->|"area"| B
    B -->|"area"| A
```

### 3.6 Relative Motion in 1D

Velocities add in one dimension:
$$v_{AC} = v_{AB} + v_{BC}$$

---

## 4 | Common Problem Types

### Type 1: Braking distance (constant deceleration)
> A car at $20\ \text{m/s}$ brakes at $-5\ \text{m/s}^2$. Find stopping distance.

**Solution:** Using $v^2 = v_0^2 + 2a\Delta x$ with $v = 0$:
$$0 = 20^2 + 2(-5)\Delta x \Rightarrow \Delta x = \frac{400}{10} = 40\ \text{m}$$

### Type 2: Free fall — dropped object
> A ball is dropped from $45\ \text{m}$. Find the time to hit the ground.

**Solution:**
$$y = \frac{1}{2}gt^2 \Rightarrow t = \sqrt{\frac{2y}{g}} = \sqrt{\frac{90}{9.8}} \approx 3.03\ \text{s}$$

### Type 3: Projectile launched at an angle
> A ball is kicked at $15\ \text{m/s}$ at $30^\circ$. Find range and max height.

**Solution:**
$$v_{0x} = 15\cos 30^\circ = 13.0, \quad v_{0y} = 15\sin 30^\circ = 7.5$$
$$R = \frac{v_0^2 \sin 2\theta}{g} = \frac{225 \sin 60^\circ}{9.8} \approx 19.9\ \text{m}$$
$$H = \frac{v_{0y}^2}{2g} = \frac{56.25}{19.6} \approx 2.87\ \text{m}$$

### Type 4: Interpreting a velocity-time graph
> A $v$-$t$ graph is linear from $0$ to $10\ \text{m/s}$ in $5\ \text{s}$, then constant. Find acceleration and distance.

**Solution:**
$$a = \frac{10 - 0}{5} = 2\ \text{m/s}^2$$
Distance (area): triangle + rectangle
$$\text{Area} = \frac{1}{2}(5)(10) + (10-5)(10) = 25 + 50 = 75\ \text{m}$$

---

## 5 | Cross-Links

- [[01_Measurement_and_Scientific_Method]] — units and uncertainty in kinematic data
- [[03_Dynamics]] — forces cause the accelerations described here
- [[01_Advance Mathematics (Sci-Math) - Overview|Mathematics]] — vectors, trigonometry, quadratic equations
