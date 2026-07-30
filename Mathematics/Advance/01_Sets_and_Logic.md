---
tags:
  - mathematics
  - advance
  - sets
  - logic
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค301"]
---

# Sets and Logic — เซตและตรรกศาสตร์

> *"Logic is the beginning of wisdom, not the end. Sets provide the language; logic provides the rules."*

Sets and Logic form the foundational language of mathematics at the high school level. Students learn to precisely describe collections of objects, perform operations on sets, and reason about propositions using formal logical connectives. This topic bridges the informal set theory from ม.1–3 and prepares students for proof-based mathematics.

---

## 1 | Course Coverage

### ม.4 (ค301)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Set theory review and extension | Set operations (union, intersection, complement, difference); power sets; Cartesian products; counting principles for sets; inclusion-exclusion for 2 and 3 sets |
| **Semester 1** | Propositional logic | Propositions (ประพจน์); logical connectives (∧, ∨, →, ↔, ~); truth tables; tautologies and contradictions; logical equivalence |
| **Semester 1** | Predicates and quantifiers | Open sentences (ประโยคเปิด); universal quantifier (∀); existential quantifier (∃); negating quantified statements |
| **Semester 1** | Arguments and validity | Valid and invalid arguments; rules of inference; direct and indirect reasoning |

---

## 2 | Key Terminology

| Thai | English | Symbol |
|---|---|---|
| เซต | Set | { } |
| สมาชิก | Element | ∈ |
| เอกภพสัมพัทธ์ | Universal set | U |
| เซตว่าง | Empty set | ∅ |
| สับเซต | Subset | ⊂ |
| เพาเวอร์เซต | Power set | P(A) |
| ผลคูณคาร์ทีเซียน | Cartesian product | A × B |
| ยูเนียน | Union | ∪ |
| อินเตอร์เซกชัน | Intersection | ∩ |
| คอมพลีเมนต์ | Complement | A' |
| ประพจน์ | Proposition | p, q, r |
| ตัวเชื่อม | Connective | ∧, ∨, →, ↔, ~ |
| ตารางค่าความจริง | Truth table | — |
| สัจนิรันดร์ | Tautology | Always true |
| ข้อขัดแย้ง | Contradiction | Always false |
| สมมูล | Logical equivalence | ≡ |
| ประโยคเปิด | Open sentence | P(x) |
| ตัวบ่งปริมาณ | Quantifier | ∀, ∃ |

---

## 3 | Key Concepts

### 3.1 Set Operations Review

**Cardinality formula for two sets:**
$$n(A \cup B) = n(A) + n(B) - n(A \cap B)$$

**For three sets:**
$$n(A \cup B \cup C) = n(A) + n(B) + n(C) - n(A \cap B) - n(A \cap C) - n(B \cap C) + n(A \cap B \cap C)$$

### 3.2 Power Sets

The power set P(A) is the set of all subsets of A.

$$\text{If } n(A) = k, \text{ then } n(P(A)) = 2^k$$

**Example:** A = {1, 2}
$$P(A) = \{\emptyset, \{1\}, \{2\}, \{1, 2\}\}$$
$$n(P(A)) = 2^2 = 4$$

### 3.3 Cartesian Products

$$A \times B = \{(a, b) \mid a \in A \text{ and } b \in B\}$$

**Cardinality:**
$$n(A \times B) = n(A) \times n(B)$$

**Example:** A = {1, 2}, B = {x, y, z}
$$A \times B = \{(1,x), (1,y), (1,z), (2,x), (2,y), (2,z)\}$$

### 3.4 Logical Connectives

| Connective | Symbol | Name | True when |
|---|---|---|---|
| Conjunction | p ∧ q | AND | Both p and q are true |
| Disjunction | p ∨ q | OR | At least one is true |
| Implication | p → q | If...then | False only when p is true and q is false |
| Biconditional | p ↔ q | If and only if | Both have same truth value |
| Negation | ~p | NOT | Opposite of p |

**Truth table for implication (most important):**

| p | q | p → q |
|---|---|---|
| T | T | T |
| T | F | **F** |
| F | T | T |
| F | F | T |

> **Key insight:** An implication is false ONLY when the hypothesis is true but the conclusion is false.

### 3.5 Logical Equivalence

Two propositions are logically equivalent (≡) if they have identical truth tables.

**Key equivalences:**
- De Morgan's Laws:
  - $~(p \land q) \equiv ~p \lor ~q$
  - $~(p \lor q) \equiv ~p \land ~q$
- Contrapositive: $p \to q \equiv ~q \to ~p$
- Implication: $p \to q \equiv ~p \lor q$

### 3.6 Quantifiers

**Universal quantifier (∀):** "For all"
$$\forall x \in \mathbb{R}, x^2 \geq 0$$
"For all real numbers x, x squared is non-negative."

**Existential quantifier (∃):** "There exists"
$$\exists x \in \mathbb{Z}, x^2 = 4$$
"There exists an integer x such that x squared equals 4."

**Negating quantified statements:**
$$~(\forall x, P(x)) \equiv \exists x, ~P(x)$$
$$~(\exists x, P(x)) \equiv \forall x, ~P(x)$$

**Example:** 
- Statement: "All students passed the exam" (∀x, P(x))
- Negation: "There exists a student who did not pass" (∃x, ~P(x))

---

## 4 | Common Problem Types

### Type 1: Power Set Cardinality
> If A has 5 elements, how many subsets does A have?

**Solution:** $n(P(A)) = 2^5 = 32$ subsets

### Type 2: Cartesian Product
> A = {1, 2, 3}, B = {a, b}. Find A × B and n(A × B).

**Solution:** 
$$A \times B = \{(1,a), (1,b), (2,a), (2,b), (3,a), (3,b)\}$$
$$n(A \times B) = 3 \times 2 = 6$$

### Type 3: Truth Table Construction
> Construct a truth table for $(p \to q) \land ~p$.

**Solution:**

| p | q | p → q | ~p | (p → q) ∧ ~p |
|---|---|---|---|---|
| T | T | T | F | F |
| T | F | F | F | F |
| F | T | T | T | T |
| F | F | T | T | T |

### Type 4: Logical Equivalence
> Show that $p \to q \equiv ~q \to ~p$ (contrapositive).

**Solution:** Construct truth tables for both and verify they match.

### Type 5: Negating Quantified Statements
> Negate: "Every even number is divisible by 4."

**Solution:** "There exists an even number that is not divisible by 4."
(Example: 6 is even but not divisible by 4)

### Type 6: Venn Diagram Problem (3 sets)
> In a survey of 100 students: 60 like math, 50 like science, 40 like English, 30 like both math and science, 20 like both math and English, 15 like both science and English, 10 like all three. How many like at least one subject?

**Solution:**
$$n(M \cup S \cup E) = 60 + 50 + 40 - 30 - 20 - 15 + 10 = 95$$
So **95 students** like at least one subject.

---

## 5 | Cross-Links

- [[Fundamental/17_Sets]] — Foundation from ม.1–3
- [[02_Real_Numbers_and_Inequalities]] — Solution sets of inequalities
- [[05_Functions]] — Functions as relations (subsets of Cartesian products)
- [[21_Mathematical_Reasoning]] — Proof techniques build on logic
