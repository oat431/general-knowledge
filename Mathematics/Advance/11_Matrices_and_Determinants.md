---
tags:
  - mathematics
  - advance
  - matrices
  - determinants
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค302"]
---

# Matrices and Determinants — เมทริกซ์และดีเทอร์มิแนนต์

> *"Matrices are the language of linear systems — compact, powerful, and universally applicable."*

Matrices provide a systematic way to organize and manipulate data, solve systems of equations, and represent linear transformations. This topic covers matrix operations, determinants, inverses, and their applications to solving systems — foundational for computer graphics, data science, engineering, and physics.

---

## 1 | Course Coverage

### ม.5 (ค302)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Matrix basics | Definition; dimensions; types (square, row, column, zero, identity); equality |
| **Semester 1** | Matrix operations | Addition, subtraction, scalar multiplication, matrix multiplication |
| **Semester 1** | Determinants | 2×2 and 3×3 determinants; properties; cofactor expansion |
| **Semester 1** | Matrix inverse | Conditions for invertibility; formula for 2×2; adjoint method for 3×3 |
| **Semester 1** | Systems of equations | Matrix equation $AX = B$; solving via $X = A^{-1}B$; Cramer's rule |
| **Semester 1** | Row operations | Gaussian elimination; row echelon form |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| เมทริกซ์ | Matrix | $A$, $B$, $[a_{ij}]$ |
| มิติ | Dimensions | $m \times n$ |
| เมทริกซ์จัตุรัส | Square matrix | $n \times n$ |
| เมทริกซ์เอกลักษณ์ | Identity matrix | $I_n$ |
| เมทริกซ์สลับเปลี่ยน | Transpose | $A^T$ |
| ดีเทอร์มิแนนต์ | Determinant | $\det(A)$ or $|A|$ |
| เมทริกซ์ผกผัน | Inverse matrix | $A^{-1}$ |
| แอดจอينت | Adjoint | $\text{adj}(A)$ |
| กฎของแครเมอร์ | Cramer's Rule | Using determinants to solve |
| การดำเนินการตามแถว | Row operations | Elementary row operations |

---

## 3 | Key Concepts

### 3.1 Matrix Definition

An $m \times n$ matrix has $m$ rows and $n$ columns:

$$A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}$$

**Special matrices:**
- **Row matrix:** $1 \times n$
- **Column matrix:** $m \times 1$
- **Square matrix:** $n \times n$
- **Zero matrix:** All entries are 0
- **Identity matrix ($I_n$):** Diagonal entries are 1, rest are 0

### 3.2 Matrix Operations

**Addition/Subtraction:** (same dimensions only)
$$[a_{ij}] + [b_{ij}] = [a_{ij} + b_{ij}]$$

**Scalar multiplication:**
$$c[a_{ij}] = [ca_{ij}]$$

**Matrix multiplication:** $C = AB$ where $A$ is $m \times p$ and $B$ is $p \times n$
$$c_{ij} = \sum_{k=1}^p a_{ik} b_{kj}$$

> **Important:** Matrix multiplication is NOT commutative: $AB \neq BA$ in general.

**Properties:**
- $A + B = B + A$ (commutative)
- $(AB)C = A(BC)$ (associative)
- $A(B + C) = AB + AC$ (distributive)
- $IA = AI = A$ (identity)

### 3.3 Determinants

**2×2 determinant:**
$$\det\begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc$$

**3×3 determinant (cofactor expansion along first row):**
$$\det\begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix} = a(ei - fh) - b(di - fg) + c(dh - eg)$$

**Properties:**
- $\det(AB) = \det(A) \cdot \det(B)$
- $\det(A^T) = \det(A)$
- Swapping two rows changes the sign
- If a row is all zeros, $\det = 0$
- If two rows are identical, $\det = 0$

### 3.4 Matrix Inverse

**For 2×2:**
$$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \Rightarrow A^{-1} = \frac{1}{ad - bc}\begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

**Existence:** $A^{-1}$ exists if and only if $\det(A) \neq 0$.

**Properties:**
- $AA^{-1} = A^{-1}A = I$
- $(AB)^{-1} = B^{-1}A^{-1}$
- $(A^T)^{-1} = (A^{-1})^T$

### 3.5 Solving Systems with Matrices

**System:** $AX = B$

If $A$ is invertible: $X = A^{-1}B$

**Example:**
$$\begin{cases} 2x + 3y = 7 \\ x - y = 1 \end{cases}$$

$$\begin{bmatrix} 2 & 3 \\ 1 & -1 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 7 \\ 1 \end{bmatrix}$$

$\det(A) = -2 - 3 = -5$

$$A^{-1} = \frac{1}{-5}\begin{bmatrix} -1 & -3 \\ -1 & 2 \end{bmatrix} = \begin{bmatrix} 1/5 & 3/5 \\ 1/5 & -2/5 \end{bmatrix}$$

$$X = A^{-1}B = \begin{bmatrix} 1/5 & 3/5 \\ 1/5 & -2/5 \end{bmatrix}\begin{bmatrix} 7 \\ 1 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

**Solution:** $x = 2, y = 1$

### 3.6 Cramer's Rule

For system $AX = B$ where $A$ is $n \times n$ and $\det(A) \neq 0$:

$$x_i = \frac{\det(A_i)}{\det(A)}$$

where $A_i$ is $A$ with column $i$ replaced by $B$.

**Example:**
$$\begin{cases} 2x + y = 5 \\ x + 3y = 7 \end{cases}$$

$D = \det\begin{bmatrix} 2 & 1 \\ 1 & 3 \end{bmatrix} = 5$

$D_x = \det\begin{bmatrix} 5 & 1 \\ 7 & 3 \end{bmatrix} = 8$

$D_y = \det\begin{bmatrix} 2 & 5 \\ 1 & 7 \end{bmatrix} = 9$

$x = 8/5$, $y = 9/5$

---

## 4 | Common Problem Types

### Type 1: Matrix Multiplication
> Compute $AB$ where $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$, $B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}$.

**Solution:** $AB = \begin{bmatrix} 1(5)+2(7) & 1(6)+2(8) \\ 3(5)+4(7) & 3(6)+4(8) \end{bmatrix} = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}$

### Type 2: Determinant
> Find $\det\begin{bmatrix} 2 & -1 & 3 \\ 0 & 4 & 1 \\ 5 & 2 & -1 \end{bmatrix}$.

**Solution:** Expand along row 1:
$2(4(-1) - 1(2)) - (-1)(0(-1) - 1(5)) + 3(0(2) - 4(5))$
$= 2(-6) + 1(-5) + 3(-20) = -12 - 5 - 60 = -77$

### Type 3: Matrix Inverse
> Find the inverse of $\begin{bmatrix} 3 & 1 \\ 2 & 4 \end{bmatrix}$.

**Solution:** $\det = 12 - 2 = 10$
$A^{-1} = \frac{1}{10}\begin{bmatrix} 4 & -1 \\ -2 & 3 \end{bmatrix} = \begin{bmatrix} 2/5 & -1/10 \\ -1/5 & 3/10 \end{bmatrix}$

### Type 4: Solving System with Matrix
> Solve $\begin{cases} x + 2y = 4 \\ 3x - y = 5 \end{cases}$ using matrix method.

**Solution:** $A = \begin{bmatrix} 1 & 2 \\ 3 & -1 \end{bmatrix}$, $\det = -7$
$A^{-1} = \frac{1}{-7}\begin{bmatrix} -1 & -2 \\ -3 & 1 \end{bmatrix} = \begin{bmatrix} 1/7 & 2/7 \\ 3/7 & -1/7 \end{bmatrix}$
$X = A^{-1}\begin{bmatrix} 4 \\ 5 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$

### Type 5: Cramer's Rule (3 variables)
> Solve $\begin{cases} x + y + z = 6 \\ 2x - y + z = 3 \\ x + 2y - z = 2 \end{cases}$

**Solution:** $D = 3$, $D_x = 3$, $D_y = 6$, $D_z = 9$
$x = 1, y = 2, z = 3$

---

## 5 | Cross-Links

- [[04_Systems_of_Equations]] — Matrix methods for solving
- [[10_Complex_Numbers]] — Complex matrices
- [[13_Vectors]] — Matrices as transformations
- [[01_Sets_and_Logic]] — Matrix algebra structure
