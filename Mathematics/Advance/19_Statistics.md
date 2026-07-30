---
tags:
  - mathematics
  - advance
  - statistics
  - regression
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค303"]
---

# Statistics — สถิติ

> *"Statistics is the science of learning from data — turning numbers into knowledge."*

Statistics extends basic data handling to inferential methods: drawing conclusions about populations from samples. This topic covers measures of central tendency and dispersion, correlation, regression, sampling methods, and hypothesis testing.

---

## 1 | Course Coverage

### ม.6 (ค303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Descriptive statistics review | Mean, median, mode; variance, standard deviation; quartiles |
| **Semester 1** | Correlation | Scatter plots; Pearson correlation coefficient $r$; interpretation |
| **Semester 1** | Linear regression | Least squares line; prediction; residual analysis |
| **Semester 1** | Sampling methods | Simple random; stratified; systematic; cluster; bias |
| **Semester 1** | Sampling distributions | Distribution of sample mean; Central Limit Theorem |
| **Semester 1** | Hypothesis testing | Null and alternative hypotheses; test statistics; p-values; z-test and t-test (intro) |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| ประชากร | Population | $N$ |
| กลุ่มตัวอย่าง | Sample | $n$ |
| ค่าเฉลี่ย | Mean | $\bar{x}$, $\mu$ |
| มัธยฐาน | Median | $\tilde{x}$ |
| ฐานนิยม | Mode | — |
| ความแปรปรวน | Variance | $s^2$, $\sigma^2$ |
| ส่วนเบี่ยงเบนมาตรฐาน | Standard deviation | $s$, $\sigma$ |
| ควอร์ไทล์ | Quartile | $Q_1, Q_2, Q_3$ |
| สหสัมพันธ์ | Correlation | $r$ |
| การถดถอย | Regression | $\hat{y} = a + bx$ |
| สมมุติฐานว่าง | Null hypothesis | $H_0$ |
| สมมุติฐานทางเลือก | Alternative hypothesis | $H_1$ or $H_a$ |
| ค่า p | p-value | — |

---

## 3 | Key Concepts

### 3.1 Measures of Central Tendency

**Mean:**
$$\bar{x} = \frac{\sum x_i}{n}$$

**Median:** Middle value when data is sorted.

**Mode:** Most frequent value.

### 3.2 Measures of Dispersion

**Range:** $\max - \min$

**Variance (sample):**
$$s^2 = \frac{\sum(x_i - \bar{x})^2}{n - 1}$$

**Standard deviation:**
$$s = \sqrt{s^2}$$

**Coefficient of variation:**
$$CV = \frac{s}{\bar{x}} \times 100\%$$

### 3.3 Quartiles and Box Plots

- $Q_1$: 25th percentile
- $Q_2$: 50th percentile (median)
- $Q_3$: 75th percentile
- **IQR** = $Q_3 - Q_1$
- **Outlier:** Below $Q_1 - 1.5 \times \text{IQR}$ or above $Q_3 + 1.5 \times \text{IQR}$

### 3.4 Correlation

**Pearson correlation coefficient:**
$$r = \frac{n\sum xy - \sum x \sum y}{\sqrt{[n\sum x^2 - (\sum x)^2][n\sum y^2 - (\sum y)^2]}}$$

| $r$ value | Interpretation |
|---|---|
| $r = +1$ | Perfect positive correlation |
| $0 < r < 1$ | Positive correlation |
| $r = 0$ | No linear correlation |
| $-1 < r < 0$ | Negative correlation |
| $r = -1$ | Perfect negative correlation |

### 3.5 Linear Regression

**Least squares regression line:**
$$\hat{y} = a + bx$$

where:
$$b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - (\sum x)^2}$$
$$a = \bar{y} - b\bar{x}$$

**Coefficient of determination:**
$$r^2 = \text{proportion of variation in } y \text{ explained by } x$$

### 3.6 Central Limit Theorem

For samples of size $n$ from a population with mean $\mu$ and standard deviation $\sigma$:

$$\bar{X} \sim N\left(\mu, \frac{\sigma^2}{n}\right)$$

(approximately, for large $n$ — typically $n \geq 30$)

### 3.7 Hypothesis Testing

**Steps:**
1. State $H_0$ and $H_1$
2. Choose significance level $\alpha$ (typically 0.05)
3. Calculate test statistic
4. Find p-value or critical value
5. Decision: Reject $H_0$ if p-value $< \alpha$

**Z-test for population mean (known $\sigma$):**
$$z = \frac{\bar{x} - \mu_0}{\sigma / \sqrt{n}}$$

---

## 4 | Common Problem Types

### Type 1: Mean and Standard Deviation
> Find mean and standard deviation of: $4, 8, 6, 10, 2$.

**Solution:**
$\bar{x} = 30/5 = 6$
Deviations: $-2, 2, 0, 4, -4$. Squared: $4, 4, 0, 16, 16$
$s^2 = 40/4 = 10$, $s = \sqrt{10} \approx 3.16$

### Type 2: Correlation
> Given $\sum x = 50$, $\sum y = 80$, $\sum xy = 420$, $\sum x^2 = 300$, $\sum y^2 = 700$, $n = 10$. Find $r$.

**Solution:**
$r = \frac{10(420) - 50(80)}{\sqrt{[10(300) - 2500][10(700) - 6400]}} = \frac{200}{\sqrt{500 \times 600}} = \frac{200}{\sqrt{300000}} \approx 0.365$

### Type 3: Regression Line
> Find the regression line for the data above.

**Solution:**
$b = \frac{200}{500} = 0.4$
$a = 8 - 0.4(5) = 6$
$\hat{y} = 6 + 0.4x$

### Type 4: Central Limit Theorem
> Population has $\mu = 50$, $\sigma = 10$. For samples of size $n = 25$, find $P(\bar{X} > 53)$.

**Solution:** $\bar{X} \sim N(50, 4)$. $\sigma_{\bar{x}} = 10/5 = 2$
$z = \frac{53-50}{2} = 1.5$
$P(Z > 1.5) = 1 - 0.9332 = 0.0668$

### Type 5: Hypothesis Test
> A factory claims bulbs last $\mu = 1000$ hours. A sample of 36 bulbs has $\bar{x} = 980$, $s = 60$. Test at $\alpha = 0.05$.

**Solution:**
$H_0: \mu = 1000$ vs $H_1: \mu < 1000$
$z = \frac{980 - 1000}{60/\sqrt{36}} = \frac{-20}{10} = -2$
p-value $= P(Z < -2) = 0.0228 < 0.05$
**Reject $H_0$.** There is evidence the mean is less than 1000 hours.

---

## 5 | Cross-Links

- [[Fundamental/18_Statistics_Data_Handling]] — Basic statistics foundation
- [[18_Probability_Distributions]] — Normal distribution in inference
- [[17_Probability]] — Probability basis for inference
