---
tags:
  - mathematics
  - cheatsheet
  - roadmap
level: "Meta: the map of all maps"
sources: ["[[00_Index]]"]
created: 2026-10-02
---

# Math Roadmap: From Counting Numbers to Calculus

> *"The board on the box lid: every piece, where it goes, and in what order you unlock it."*

This roadmap shows the entire journey as **one dependency map**: each node is a topic, each arrow means "learn this first". Click any node to jump to its cheat sheet rulebook.

---

## The Full Map

```mermaid
flowchart TD
    subgraph S0["Stage 0: Number Foundation (Zero)"]
        N1["Counting Numbers<br/>and Numeration"] --> N2["Four Operations<br/>+ - x ÷"]
        N2 --> N3["Factors, Multiples<br/>GCD and LCM"]
        N2 --> N4["Integers<br/>Negative Numbers"]
        N4 --> N5["Fractions"]
        N5 --> N6["Decimals"]
        N6 --> N7["Percentages"]
        N5 --> N8["Ratios and<br/>Proportions"]
    end

    subgraph S1["Stage 1: The Language of Math"]
        A1["Patterns and<br/>Algebraic Thinking"] --> A2["Variables and<br/>Expressions"]
        A2 --> A3["Linear Equations"]
        A3 --> A4["Quadratic Equations<br/>and Factoring"]
        A3 --> A5["Systems of<br/>Equations"]
        A4 --> A6["Inequalities"]
        A2 --> A7["Exponents and<br/>Radicals"]
        A7 --> A8["Functions"]
        A8 --> A9["Exponential and<br/>Log Functions"]
        A9 --> A10["Sequences and Series<br/>Compound Interest"]
    end

    subgraph S2["Stage 2: Space and Measure"]
        G1["Shapes and Angles"] --> G2["Perimeter<br/>and Area"]
        G2 --> G3["Volume and<br/>Surface Area"]
        G1 --> G4["Pythagoras and<br/>Right Triangles"]
        G4 --> G5["Right-Triangle<br/>Trigonometry<br/>SOH-CAH-TOA"]
        N8 --> G6["Measurement and<br/>Unit Conversion"]
        A3 --> G7["Coordinate Plane<br/>Distance, Slope"]
        G7 --> G5
    end

    subgraph S3["Stage 3: Data and Uncertainty"]
        D1["Data Types and<br/>Graphs"] --> D2["Mean, Median<br/>Mode, Range"]
        D2 --> D3["Variance and<br/>Standard Deviation"]
        D3 --> D4["Normal Distribution<br/>z-Scores"]
        N3 --> D5["Counting Rules<br/>Permutation, Combination"]
        D5 --> D6["Probability Rules"]
        D6 --> D7["Distributions and<br/>Expected Value"]
        D4 --> D7
    end

    subgraph S4["Stage 4: The Rulebook about Rulebooks"]
        L1["Sets"] --> L2["Set Operations<br/>Venn Diagrams"]
        L2 --> L3["Logic Connectives<br/>Truth Tables"]
        L3 --> L4["Proof Methods<br/>Direct, Contrapositive,<br/>Contradiction"]
        L4 --> L5["Problem-Solving<br/>Processes"]
    end

    subgraph S5["Stage 5: Calculus, the Expansion Pack"]
        C1["Limits and<br/>Continuity"] --> C2["Derivatives"]
        C2 --> C3["Applications:<br/>Optimization,<br/>Related Rates"]
        C2 --> C4["Integrals"]
        C4 --> C5["FTC, Area<br/>and Volume"]
        C4 --> C6["Differential<br/>Equations"]
    end

    N7 --> A1
    A6 --> C1
    A8 --> C1
    A9 --> C1
    G5 --> C1
    L4 --> C1

    click N1 "[[01_Numbers_and_Arithmetic]]"
    click N2 "[[01_Numbers_and_Arithmetic]]"
    click N3 "[[01_Numbers_and_Arithmetic]]"
    click N4 "[[01_Numbers_and_Arithmetic]]"
    click N5 "[[01_Numbers_and_Arithmetic]]"
    click N6 "[[01_Numbers_and_Arithmetic]]"
    click N7 "[[01_Numbers_and_Arithmetic]]"
    click N8 "[[01_Numbers_and_Arithmetic]]"
    click A1 "[[02_Algebra_and_Functions]]"
    click A2 "[[02_Algebra_and_Functions]]"
    click A3 "[[02_Algebra_and_Functions]]"
    click A4 "[[02_Algebra_and_Functions]]"
    click A5 "[[02_Algebra_and_Functions]]"
    click A6 "[[02_Algebra_and_Functions]]"
    click A7 "[[02_Algebra_and_Functions]]"
    click A8 "[[02_Algebra_and_Functions]]"
    click A9 "[[02_Algebra_and_Functions]]"
    click A10 "[[02_Algebra_and_Functions]]"
    click G1 "[[03_Geometry_and_Measurement]]"
    click G2 "[[03_Geometry_and_Measurement]]"
    click G3 "[[03_Geometry_and_Measurement]]"
    click G4 "[[03_Geometry_and_Measurement]]"
    click G5 "[[03_Geometry_and_Measurement]]"
    click G6 "[[03_Geometry_and_Measurement]]"
    click G7 "[[03_Geometry_and_Measurement]]"
    click D1 "[[04_Data_Probability_and_Statistics]]"
    click D2 "[[04_Data_Probability_and_Statistics]]"
    click D3 "[[04_Data_Probability_and_Statistics]]"
    click D4 "[[04_Data_Probability_and_Statistics]]"
    click D5 "[[04_Data_Probability_and_Statistics]]"
    click D6 "[[04_Data_Probability_and_Statistics]]"
    click D7 "[[04_Data_Probability_and_Statistics]]"
    click L1 "[[05_Sets_Logic_and_Processes]]"
    click L2 "[[05_Sets_Logic_and_Processes]]"
    click L3 "[[05_Sets_Logic_and_Processes]]"
    click L4 "[[05_Sets_Logic_and_Processes]]"
    click L5 "[[05_Sets_Logic_and_Processes]]"
    click C1 "[[06_Calculus]]"
    click C2 "[[06_Calculus]]"
    click C3 "[[06_Calculus]]"
    click C4 "[[06_Calculus]]"
    click C5 "[[06_Calculus]]"
    click C6 "[[06_Calculus]]"

    style S0 fill:#1FB85422,stroke:#1FB854
    style S1 fill:#1EB88E22,stroke:#1EB88E
    style S2 fill:#1FB8AB22,stroke:#1FB8AB
    style S3 fill:#1FB85422,stroke:#1FB854
    style S4 fill:#1EB88E22,stroke:#1EB88E
    style S5 fill:#1FB8AB22,stroke:#1FB8AB
```

---

## The Same Journey as a Ladder

```mermaid
flowchart LR
    Z["🔢 Stage 0<br/>Numbers<br/>01"] --> L["🔤 Stage 1<br/>Algebra<br/>02"]
    L --> S["📐 Stage 2<br/>Geometry<br/>03"]
    L --> D["📊 Stage 3<br/>Data<br/>04"]
    S --> R["🧠 Stage 4<br/>Sets and Logic<br/>05"]
    D --> R
    R --> C["∞ Stage 5<br/>Calculus<br/>06"]

    click Z "[[01_Numbers_and_Arithmetic]]"
    click L "[[02_Algebra_and_Functions]]"
    click S "[[03_Geometry_and_Measurement]]"
    click D "[[04_Data_Probability_and_Statistics]]"
    click R "[[05_Sets_Logic_and_Processes]]"
    click C "[[06_Calculus]]"

    style Z fill:#1FB854,color:#fff
    style L fill:#1EB88E,color:#fff
    style S fill:#1FB8AB,color:#fff
    style D fill:#1FB854,color:#fff
    style R fill:#1EB88E,color:#fff
    style C fill:#1FB8AB,color:#fff
```

**The 5 unlock gates into Calculus** (arrows converging on Limits):

| Gate | Unlocked by | Rulebook |
|---|---|---|
| Algebra fluency | Equations, inequalities, functions | [[02_Algebra_and_Functions]] |
| Function shapes | Exponential, log, trig functions | [[02_Algebra_and_Functions]] |
| Right-triangle trig | SOH-CAH-TOA | [[03_Geometry_and_Measurement]] |
| Proof mindset | Logic, proof methods | [[05_Sets_Logic_and_Processes]] |
| Number maturity | Everything in Stage 0 | [[01_Numbers_and_Arithmetic]] |

---

## Stage Table

| Stage | Name | Topics | Cheat sheet | Source notes |
|---|---|---|---|---|
| 0 | Number Foundation | Numeration, operations, factors, integers, fractions, decimals, percentages, ratios | [[01_Numbers_and_Arithmetic]] | `Fundamental/01`–`09` |
| 1 | Language of Math | Patterns, expressions, equations, inequalities, functions, exponents/logs, sequences | [[02_Algebra_and_Functions]] | `Fundamental/10`–`11`, `Advance/02`–`06`, `08` |
| 2 | Space and Measure | Angles, shapes, area/volume, units, coordinates, right-triangle trig | [[03_Geometry_and_Measurement]] | `Fundamental/12`–`16`, `Advance/07` |
| 3 | Data and Uncertainty | Graphs, statistics, counting, probability, distributions | [[04_Data_Probability_and_Statistics]] | `Fundamental/18`–`19`, `Advance/17`, `19` |
| 4 | Rulebook about Rulebooks | Sets, logic, proofs, problem-solving | [[05_Sets_Logic_and_Processes]] | `Fundamental/17`, `20`, `Advance/01`, `21` |
| 5 | Calculus (expansion pack) | Limits, derivatives, integrals, differential equations | [[06_Calculus]] | `Advance/14`–`16`, `23` |

---

## How to Read This Map

1. **Follow arrows**: an arrow `X → Y` means "X is a prerequisite of Y". You may learn nodes in any order that respects the arrows.
2. **Stages are not strict**: Stage 2 and Stage 3 can be learned in parallel after Stage 1. Only Calculus waits for everything.
3. **Click a node** to open its cheat sheet rulebook; the cheat sheet's own chain links (⬅ · ➡) walk you through in reading order.
4. **The practical finish line is Stage 4**: everything up to here covers everyday math. Stage 5 is the expansion pack for science, engineering, and economics.

---

## Chain Navigation

⬅ [[00_Index]] · ➡ [[01_Numbers_and_Arithmetic]]
