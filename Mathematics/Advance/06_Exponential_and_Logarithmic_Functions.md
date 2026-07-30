---
tags:
  - mathematics
  - advance
  - exponential
  - logarithm
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Exponential and Logarithmic Functions — ฟังก์ชันเอกซ์โพเนนเชียลและลอการิทึม

> *"Exponential growth is the most powerful force in the universe — and logarithms are its decoder ring."*

Exponential and logarithmic functions model phenomena that grow or decay at rates proportional to their current value — from population growth and radioactive decay to compound interest and sound intensity. These functions are inverses of each other and form a critical bridge to calculus.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 2** | Exponential functions | Definition $f(x) = a^x$; properties of exponents; graphs; transformations |
| **Semester 2** | The number e | Natural exponential $e^x$; continuous growth; applications |
| **Semester 2** | Logarithmic functions | Definition $\log_a x$; properties; common and natural logs; graphs |
| **Semester 2** | Logarithm properties | Product, quotient, power rules; change of base formula |
| **Semester 2** | Exponential equations | Solving $a^x = b$; using logs to solve; applications |
| **Semester 2** | Logarithmic equations | Solving $\log_a x = b$; using properties; extraneous solutions |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| ฟังก์ชันเอกซ์โพเนนเชียล | Exponential function | $f(x) = a^x$ |
| ฟังก์ชันลอการิทึม | Logarithmic function | $f(x) = \log_a x$ |
| ฐาน | Base | $a$ in $a^x$ or $\log_a$ |
| ลอการิทึมสามัญ | Common logarithm | $\log_{10}$ or $\log$ |
| ลอการิทึมธรรมชาติ | Natural logarithm | $\ln$ or $\log_e$ |
| เลข e | Euler's number | $e \approx 2.71828$ |
| สูตรเปลี่ยนฐาน | Change of base formula | $\log_a x = \frac{\log_b x}{\log_b a}$ |
| ดอกเบี้ยทบต้น | Compound interest | $A = P(1 + r/n)^{nt}$ |
| การเติบโตต่อเนื่อง | Continuous growth | $A = Pe^{rt}$ |

---

## 3 | Key Concepts

### 3.1 Exponential Functions

**Definition:** $f(x) = a^x$ where $a > 0$ and $a \neq 1$

**Properties:**
- Domain: $\mathbb{R}$
- Range: $(0, \infty)$
- y-intercept: $(0, 1)$
- Horizontal asymptote: $y = 0$
- If $a > 1$: increasing (growth)
- If $0 < a < 1$: decreasing (decay)

**Laws of exponents:**
$$a^m \cdot a^n = a^{m+n}$$
$$\frac{a^m}{a^n} = a^{m-n}$$
$$(a^m)^n = a^{mn}$$
$$(ab)^n = a^n b^n$$
$$a^0 = 1$$
$$a^{-n} = \frac{1}{a^n}$$
$$a^{1/n} = \sqrt[n]{a}$$

### 3.2 The Number e

$$e = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n \approx 2.71828$$

**Natural exponential function:** $f(x) = e^x$

**Continuous compound interest:**
$$A = Pe^{rt}$$
where $P$ = principal, $r$ = annual rate, $t$ = time in years

### 3.3 Logarithmic Functions

**Definition:** $y = \log_a x$ if and only if $a^y = x$

**Properties:**
- Domain: $(0, \infty)$
- Range: $\mathbb{R}$
- x-intercept: $(1, 0)$
- Vertical asymptote: $x = 0$
- Inverse of exponential: $\log_a(a^x) = x$ and $a^{\log_a x} = x$

**Special cases:**
- $\log_{10} x = \log x$ (common log)
- $\log_e x = \ln x$ (natural log)

### 3.4 Logarithm Properties

**Product rule:**
$$\log_a(MN) = \log_a M + \log_a N$$

**Quotient rule:**
$$\log_a\left(\frac{M}{N}\right) = \log_a M - \log_a N$$

**Power rule:**
$$\log_a(M^p) = p \log_a M$$

**Change of base:**
$$\log_a x = \frac{\log_b x}{\log_b a} = \frac{\ln x}{\ln a} = \frac{\log x}{\log a}$$

### 3.5 Solving Exponential Equations

**Method 1:** Same base
$$2^x = 8 \Rightarrow 2^x = 2^3 \Rightarrow x = 3$$

**Method 2:** Take logarithm of both sides
$$3^x = 10$$
$$\ln(3^x) = \ln(10)$$
$$x \ln 3 = \ln 10$$
$$x = \frac{\ln 10}{\ln 3} \approx 2.096$$

### 3.6 Solving Logarithmic Equations

**Method:** Convert to exponential form or use properties

**Example:** $\log_2(x+1) + \log_2(x-1) = 3$

Combine: $\log_2((x+1)(x-1)) = 3$
$$\log_2(x^2 - 1) = 3$$
$$x^2 - 1 = 2^3 = 8$$
$$x^2 = 9$$
$$x = \pm 3$$

**Check for extraneous solutions:** $x = -3$ gives $\log_2(-2)$ which is undefined.
**Answer:** $x = 3$

### 3.7 Applications

**Population growth:**
$$P(t) = P_0 e^{kt}$$

**Radioactive decay:**
$$N(t) = N_0 e^{-kt}$$

**Half-life:** $t_{1/2} = \frac{\ln 2}{k}$

**Compound interest:**
$$A = P\left(1 + \frac{r}{n}\right)^{nt}$$

**pH scale:**
$$\text{pH} = -\log[H^+]$$

**Decibels:**
$$\beta = 10 \log\left(\frac{I}{I_0}\right)$$

---

## 4 | Common Problem Types

### Type 1: Exponential Equation (Same Base)
> Solve: $4^{2x-1} = 8$

**Solution:** $4^{2x-1} = 2^3 \Rightarrow (2^2)^{2x-1} = 2^3$
$2^{4x-2} = 2^3 \Rightarrow 4x - 2 = 3 \Rightarrow x = \frac{5}{4}$

### Type 2: Exponential Equation (Different Bases)
> Solve: $5^x = 100$

**Solution:** $\log(5^x) = \log(100) \Rightarrow x \log 5 = 2$
$x = \frac{2}{\log 5} \approx 2.861$

### Type 3: Logarithmic Equation
> Solve: $\ln(x) + \ln(x-1) = \ln(6)$

**Solution:** $\ln(x(x-1)) = \ln(6) \Rightarrow x^2 - x = 6$
$x^2 - x - 6 = 0 \Rightarrow (x-3)(x+2) = 0$
$x = 3$ (reject $x = -2$ as extraneous)

### Type 4: Compound Interest
> $10,000 invested at 5% compounded quarterly for 10 years. Find the final amount.

**Solution:** $A = 10000\left(1 + \frac{0.05}{4}\right)^{4 \times 10} = 10000(1.0125)^{40} \approx 16,436.19$

### Type 5: Half-Life
> A radioactive substance has a half-life of 8 days. How long until 75% has decayed?

**Solution:** 75% decayed means 25% remains: $0.25 = e^{-kt}$
$k = \frac{\ln 2}{8}$
$0.25 = e^{-\frac{\ln 2}{8} t} \Rightarrow \ln(0.25) = -\frac{\ln 2}{8} t$
$t = \frac{8 \ln(0.25)}{-\ln 2} = \frac{8 \cdot (-2\ln 2)}{\ln 2} = 16$ days

---

## 5 | Cross-Links

- [[05_Functions]] — Function properties and inverses
- [[08_Sequences_and_Series]] — Geometric sequences relate to exponential growth
- [[14_Limits_and_Continuity]] — Limits involving $e$
- [[15_Differentiation]] — Derivatives of exponential and log functions
- [[16_Integration]] — Integrals involving $1/x$
