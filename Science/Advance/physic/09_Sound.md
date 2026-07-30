---
tags:
  - physics
  - advance
  - sound
  - acoustics
  - ipst
source: "IPST (สสวท.) Physics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว301"]
---

# Sound — เสียง

> *"The science of sound is the most beautiful of all the sciences."* — Hermann von Helmholtz

Sound is a longitudinal mechanical wave that propagates through a medium by means of compressions and rarefactions. Unlike transverse waves, sound requires a material medium — it cannot travel through a vacuum. The study of sound, or acoustics, encompasses the production, propagation, reception, and perception of audible pressure waves with frequencies between approximately 20 Hz and 20,000 Hz.

In the Thai high school physics curriculum, sound builds directly upon the wave mechanics studied earlier. Students apply wave principles to real phenomena: the Doppler effect explains why a passing ambulance siren changes pitch, beats reveal interference between slightly mistuned instruments, and the decibel scale quantifies the logarithmic perception of loudness. Musical acoustics connects physics to the arts, showing how standing waves in strings and air columns determine pitch and timbre.

---

## 1 | Course Coverage

### ม.4 (ว301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Wave basics, SHM | Wave equation, superposition |
| **Semester 2** | Sound, acoustics, Doppler effect, beats, intensity/dB | Calculate speed of sound, apply Doppler formula, compute beat frequency, dB calculations |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| เสียง | Sound | Audible 20 Hz – 20 kHz |
| คลื่นตามยาว | Longitudinal wave | Compression & rarefaction |
| ความเร็วเสียง | Speed of sound | $v$ (m/s) |
| ความถี่ | Frequency | $f$ (Hz) |
| คาบ | Period | $T = 1/f$ (s) |
| ความยาวคลื่น | Wavelength | $\lambda$ (m) |
| ความเข้มเสียง | Sound intensity | $I$ (W/m²) |
| เดซิเบล | Decibel | $\beta$ (dB) |
| ปรากฏการณ์ดอปเลอร์ | Doppler effect | Frequency shift |
| การเคาะ | Beats | $f_{beat} = |f_1 - f_2|$ |
| เสียงดนตรี | Musical sound | Harmonics, overtones |
| ความดันเสียง | Sound pressure | $p$ (Pa) |

---

## 3 | Key Concepts

### 3.1 Speed of Sound

The speed of sound depends on the medium's elastic properties and density. In air at 0 °C:

$$v_{\text{air}} \approx 331 + 0.6T \quad (\text{m/s, } T \text{ in } ^\circ\text{C})$$

In general, $v = \sqrt{B/\rho}$ where $B$ is the bulk modulus and $\rho$ is density. Sound travels faster in solids than liquids, and faster in liquids than gases.

### 3.2 Sound Intensity and Decibels

Sound intensity is power per unit area:

$$I = \frac{P}{4\pi r^2}$$

The decibel scale is logarithmic:

$$\beta = 10 \log_{10}\left(\frac{I}{I_0}\right), \quad I_0 = 10^{-12} \text{ W/m}^2$$

A doubling of intensity gives $\Delta \beta \approx 3$ dB. A factor of 10 in intensity gives +10 dB.

### 3.3 Doppler Effect

When source and observer are in relative motion, observed frequency changes:

$$f' = f \left(\frac{v \pm v_o}{v \mp v_s}\right)$$

Sign convention: numerator + if observer moves toward source; denominator − if source moves toward observer. When both approach, $f'$ increases; when both separate, $f'$ decreases.

### 3.4 Beats

Two sounds of slightly different frequencies produce amplitude pulsations:

$$f_{beat} = |f_1 - f_2|$$

The beat frequency equals the absolute difference. Musicians use beats to tune instruments — zero beats means matched frequencies.

### 3.5 Musical Acoustics

**Strings (fixed at both ends):** $f_n = \frac{nv}{2L}$, $n = 1, 2, 3, \ldots$

**Open pipe (open both ends):** $f_n = \frac{nv}{2L}$, same as string.

**Closed pipe (closed one end):** $f_n = \frac{(2n-1)v}{4L}$, $n = 1, 2, 3, \ldots$ — only odd harmonics.

### 3.6 Standing Waves and Resonance

Resonance occurs when driving frequency matches a natural frequency of the system. The fundamental frequency ($f_1$) is the lowest mode. Overtones are integer multiples ($f_n = n f_1$ for strings and open pipes).

---

## 4 | Common Problem Types

### Type 1: Doppler Effect Calculation
> A train whistle emits at 500 Hz while approaching a stationary observer at 30 m/s. Speed of sound = 340 m/s. What frequency is heard?

**Solution:** Source approaching, observer stationary ($v_o = 0$):

$$f' = f \left(\frac{v}{v - v_s}\right) = 500 \times \frac{340}{340 - 30} = 500 \times \frac{340}{310} \approx 548.4 \text{ Hz}$$

### Type 2: Beat Frequency
> Two tuning forks produce 440 Hz and 443 Hz. What is the beat frequency?

**Solution:**

$$f_{beat} = |443 - 440| = 3 \text{ Hz}$$

Three amplitude pulsations per second are heard.

### Type 3: Closed Pipe Resonance
> A closed pipe has length 0.5 m. Speed of sound = 340 m/s. Find the fundamental and first overtone.

**Solution:** Fundamental: $f_1 = \frac{v}{4L} = \frac{340}{4(0.5)} = 170$ Hz. Closed pipe has only odd harmonics, so first overtone: $f_3 = 3f_1 = 510$ Hz.

### Type 4: Intensity and dB
> A sound has intensity $10^{-6}$ W/m². Find the sound level in dB.

**Solution:**

$$\beta = 10 \log_{10}\left(\frac{10^{-6}}{10^{-12}}\right) = 10 \log_{10}(10^6) = 60 \text{ dB}$$

---

## 5 | Cross-Links

- [[Fundamental/08_Waves]] — Sound is an application of wave mechanics
- [[10_Heat_and_Thermodynamics]] — Temperature affects the speed of sound in air
- [[15_Electromagnetic_Waves]] — Contrast sound (mechanical) vs. EM waves (no medium needed)
- [[16_Light_and_Optics]] — Similar wave concepts applied to light
