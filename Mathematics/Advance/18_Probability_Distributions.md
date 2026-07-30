---
tags:
  - mathematics
  - advance
  - probability-distributions
  - statistics
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค303"]
---

# Probability Distributions — การแจกแจงความน่าจะเป็น

> *"A probability distribution describes the pattern of randomness — the shape of uncertainty."*

Probability distributions formalize how probabilities are assigned to outcomes. This topic covers discrete distributions (binomial, Poisson) and continuous distributions (normal), along with expected value and variance. These concepts form the backbone of statistical inference and data science.

---

## 1 | Course Coverage

### ม.6 (ค303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Random variables | Discrete vs continuous; probability distributions |
| **Semester 1** | Expected value and variance | $E(X)$, $\text{Var}(X)$, standard deviation |
| **Semester 1** | Binomial distribution | Bernoulli trials; $B(n, p)$; mean and variance |
| **Semester 1** | Poisson distribution | Rare events; rate parameter $\lambda$ |
| **Semester 1** | Normal distribution | Standard normal; z-scores; empirical rule |
| **Semester 1** | Normal approximation | Approximating binomial with normal |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| ตัวแปรสุ่ม | Random variable | $X$ |
| การแจกแจง | Distribution | — |
| การแจกแจงแบบไม่ต่อเนื่อง | Discrete distribution | PMF |
| การแจกแจงแบบต่อเนื่อง | Continuous distribution | PDF |
| ค่าคาดหวัง | Expected value / mean | $E(X)$, $\mu$ |
| ความแปรปรวน | Variance | $\text{Var}(X)$, $\sigma^2$ |
| ส่วนเบี่ยงเบนมาตรฐาน | Standard deviation | $\sigma$ |
| การแจกแจงทวินาม | Binomial distribution | $B(n, p)$ |
| การแจกแจงปัวซอง | Poisson distribution | $\text{Poisson}(\lambda)$ |
| การแจกแจงปกติ | Normal distribution | $N(\mu, \sigma^2)$ |
| ค่า z | Z-score | $z = \frac{x-\mu}{\sigma}$ |

---

## 3 | Key Concepts

### 3.1 Random Variables

A **random variable** $X$ assigns a numerical value to each outcome.

- **Discrete:** Countable values (e.g., number of heads in 3 tosses)
- **Continuous:** Any value in an interval (e.g., height, weight)

**Probability mass function (PMF):** $P(X = x)$ for discrete

**Probability density function (PDF):** $f(x)$ where $P(a \leq X \leq b) = \int_a^b f(x)\,dx$

### 3.2 Expected Value and Variance

**Expected value (mean):**
$$\mu = E(X) = \sum x \cdot P(X=x)$$

**Variance:**
$$\sigma^2 = \text{Var}(X) = E(X^2) - [E(X)]^2 = \sum x^2 P(X=x) - \mu^2$$

**Standard deviation:**
$$\sigma = \sqrt{\text{Var}(X)}$$

### 3.3 Binomial Distribution

**Conditions:**
1. Fixed number of trials $n$
2. Two outcomes (success/failure)
3. Constant probability $p$
4. Independent trials

**PMF:**
$$P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$$

**Mean and variance:**
$$\mu = np, \quad \sigma^2 = np(1-p)$$

**Example:** A coin is tossed 10 times. Find $P(X = 3$ heads$)$.

$$P(X=3) = \binom{10}{3}(0.5)^3(0.5)^7 = 120 \times \frac{1}{1024} \approx 0.117$$

### 3.4 Poisson Distribution

**Conditions:** Events occur randomly and independently at a constant average rate $\lambda$.

**PMF:**
$$P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!}$$

**Mean and variance:**
$$\mu = \lambda, \quad \sigma^2 = \lambda$$

**Example:** A call center receives 3 calls per minute on average. Find $P(X = 5$ calls in a minute$)$.

$$P(X=5) = \frac{3^5 e^{-3}}{5!} = \frac{243 \times 0.0498}{120} \approx 0.1008$$

### 3.5 Normal Distribution

**PDF:**
$$f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$$

**Properties:**
- Bell-shaped, symmetric about $\mu$
- Mean = median = mode = $\mu$
- Inflection points at $\mu \pm \sigma$
- Total area under curve = 1

**Empirical Rule (68-95-99.7):**
- $\mu \pm 1\sigma$: ~68% of data
- $\mu \pm 2\sigma$: ~95% of data
- $\mu \pm 3\sigma$: ~99.7% of data

### 3.6 Standard Normal and Z-Scores

**Standardizing:**
$$z = \frac{x - \mu}{\sigma}$$

This converts any normal distribution to $N(0, 1)$.

**Using standard normal table:**
$$P(X < x) = P\left(Z < \frac{x-\mu}{\sigma}\right)$$

**Example:** IQ scores are normally distributed with $\mu = 100$, $\sigma = 15$. Find $P(X > 130)$.

$$z = \frac{130-100}{15} = 2$$
$$P(Z > 2) = 1 - 0.9772 = 0.0228$$

So about **2.28%** have IQ above 130.

### 3.7 Normal Approximation to Binomial

When $np \geq 5$ and $n(1-p) \geq 5$:
$$B(n, p) \approx N(np, \, np(1-p))$$

With continuity correction: use $X \pm 0.5$.

---

## 4 | Common Problem Types

### Type 1: Expected Value
> A fair die is rolled. Find $E(X)$.

**Solution:** $E(X) = \frac{1+2+3+4+5+6}{6} = 3.5$

### Type 2: Binomial Probability
> A multiple-choice test has 10 questions, each with 4 choices. If guessing randomly, find $P(X = 5$ correct$)$.

**Solution:** $P(X=5) = \binom{10}{5}(0.25)^5(0.75)^5 = 252 \times 0.000977 \times 0.2373 \approx 0.0584$

### Type 3: Poisson Probability
> Errors in a book occur at 0.5 per page. Find $P(2$ errors on a page$)$.

**Solution:** $P(X=2) = \frac{0.5^2 e^{-0.5}}{2!} = \frac{0.25 \times 0.6065}{2} \approx 0.0758$

### Type 4: Z-Score
> Heights are $N(170, 100)$. Find $P(X < 160)$.

**Solution:** $z = \frac{160-170}{10} = -1$
$P(Z < -1) = 0.1587$

### Type 5: Normal Range
> Scores are $N(500, 10000)$. Find the score at the 90th percentile.

**Solution:** $\mu = 500$, $\sigma = 100$. $z_{0.90} = 1.28$
$x = 500 + 1.28(100) = 628$

### Type 6: Variance
> Given $P(X=1) = 0.3$, $P(X=2) = 0.5$, $P(X=3) = 0.2$. Find $\text{Var}(X)$.

**Solution:**
$E(X) = 1(0.3) + 2(0.5) + 3(0.2) = 1.9$
$E(X^2) = 1(0.3) + 4(0.5) + 9(0.2) = 4.1$
$\text{Var}(X) = 4.1 - 1.9^2 = 4.1 - 3.61 = 0.49$

---

## 5 | Cross-Links

- [[17_Probability]] — Foundation probability concepts
- [[19_Statistics]] — Statistical inference uses distributions
- [[16_Integration]] — Continuous distributions use integrals
- [[06_Exponential_and_Logarithmic_Functions]] — Poisson and normal use $e$
